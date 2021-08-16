[6:23 PM] Omar, Albarghuthi
    

# **THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS**
 
 ersistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.
 
Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:
 
* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
 
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
 
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

![](https://clementbuchanan.github.io/reading-notes/images/html5.jpg)
 
**What we really want is?**
 
a lot of storage space
on the client that persists beyond a page refresh
and isn’t transmitted to the server
Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.
___
## **A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5**
 
In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.
 
userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.
 
In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain. Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System), but it was limited by some of Flash’s design quirks. By 2006, with the advent of ExternalInterface in Flash 8, accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker dojox.storage. Flash gives each domain 100 KB of storage “for free.” Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).
 
In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. (We’ve previously discussed Gears in the context of providing a geolocation API in Internet Explorer.) Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables.
 
In the meantime, Brad Neuberg and others continued to hack away on dojox.storage to provide a unified interface to all these different plugins and APIs. By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.
 
As you survey these solutions, a pattern emerges: all of them are either specific to a single browser, or reliant on a third-party plugin. Despite heroic efforts to paper over the differences (in dojox.storage), they all expose radically different interfaces, have different storage limitations, and present different user experiences. So this is the problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

​[6:23 PM] Omar, Albarghuthi
    

>### **INTRODUCING HTML5 STORAGE**
 
What I will refer to as “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.
 
>### **USING HTML5 STORAGE**
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.
 
**interface Storage {​​​​​​​​**
**getter any getItem(in DOMString key);**
**setter creator void setItem(in DOMString key, in any data);**
**}​​​​​​​​;**
 
**Calling setItem()** with a named key that already exists will silently overwrite the previous value. **Calling getItem()** with a non-existent key will return null rather than throw an exception.
 
Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the **getItem()** and **setItem()** methods, you can simply use square brackets. For example, this snippet of code:
 
**var foo = localStorage.getItem("bar");**
 
**// ...**
 
**localStorage.setItem("bar", foo);**
 
**…could be rewritten to use square bracket syntax instead:**
 
**var foo = localStorage["bar"];**
 
**// ...**
 
**localStorage["bar"] = foo;**
 
___
 
>## **TRACKING CHANGES TO THE HTML5 STORAGE AREA**
 
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever **setItem**(), **removeItem**(), or **clear**() is called and actually changes something. For example, if you set an item to its existing value or call **clear**() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.
 
The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)
 
>## **LIMITATIONS IN CURRENT BROWSERS**
 
In talking about the history of local storage hacks using third-party plugins, I made a point of mentioning the limitations of each technique, such as storage limits. I just realized that I haven’t mentioned anything about the limitations of the now-standardized HTML5 Storage. I’ll give you the answers first, then explain them. The answers, in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”
 
“5 megabytes” is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification. One thing to keep in mind is that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up. Each digit in that float is being stored as a character, not in the usual representation of a floating point number.

![](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/HTML_and_CSS/css-message-devtools.png)
 
>## **HTML5 STORAGE IN ACTION**
 
Let’s see HTML5 Storage in action. Recall the Halma game we constructed in the canvas chapter. There’s a small problem with the game: if you close the browser window mid-game, you’ll lose your progress. But with HTML5 Storage, we can save the progress locally, within the browser itself. Here is a live demonstration. Make a few moves, then close the browser tab, then re-open it. If your browser supports HTML5 Storage, the demonstration page should magically remember your exact position within the game, including the number of moves you’ve made, the position of each of the pieces on the board, and even whether a particular piece is selected.
 
How does it work? Every time a change occurs within the game, we call this function:
 
function saveGameState() {​​​​​​​​
 
    if (!supportsLocalStorage()) {​​​​​​​​ return false; }​​​​​​​​
 
    localStorage["halma.game.in.progress"] = gGameInProgress;
 
    for (var i = 0; i < kNumPieces; i++) {​​​​​​​​

    localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
 
    localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }​​​​​​​​

    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;}​​​​​​​​
 
As you can see, it uses the localStorage object to save whether there is a game in progress (gGameInProgress, a Boolean). If so, it iterates through the pieces (gPieces, a JavaScript Array) and saves the row and column number of each piece. Then it saves some additional game state, including which piece is selected (gSelectedPieceIndex, an integer), whether the piece is in the middle of a potentially long series of hops (gSelectedPieceHasMoved, a Boolean), and the total number of moves made so far (gMoveCount, an integer).


# TRACKING CHANGES TO THE HTML5 STORAGE AREA
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)

if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
The handle_storage callback function will be called with a StorageEvent object, except in Internet Explorer where the event object is stored in window.event.

function handle_storage(e) {
  if (!e) { e = window.event; }
}
At this point, the variable e will be a StorageEvent object, which has the following useful properties
