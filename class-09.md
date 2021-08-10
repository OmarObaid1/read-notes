# forms
### Why Forms?
The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.
In addition to enabling users to
search, forms also allow users
to perform other functions
online. You will see forms
when registering as a member
of a website, when shopping
online, and when signing up for
newsletters or mailing lists.


![](https://www.htmlgoodies.com/wp-content/uploads/2021/04/HTML-Form.png)

# Form Structure
<-form>
Form controls live inside a
## <-form> 
element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
action
Every <-form> element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.
## method
Forms can be sent using one of
two methods: get or post


![](https://docs.smartfor.ms/download/attachments/852294/data%20entry%20page.PNG?version=1&modificationDate=1519885273086&api=v2&effects=border-simple,blur-border)

# Text Input
## <-input>
The <-input> element is used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating.
## type="text"
When the type attribute has a
value of text, it creates a singleline text input.
name
When users enter information
into a form, the server needs to
know which form control each
piece of data was entered into.
(For example, in a login form, the
server needs to know what has
been entered as the username
and what has been given as the
password.) Therefore, each form
control requires a name attribute.
The value of this attribute
identifies the form control and is
sent along with the information
they enter to the server.
## maxlength
You can use the maxlength
attribute to limit the number
of characters a user may enter
into the text field. Its value is the
number of characters they may
enter. For example, if you were
asking for a year, the maxlength
attribute could have a value of 4.


![](https://media.geeksforgeeks.org/wp-content/uploads/20190529152440/html-input-type-text.png)

# Password Input
## <-input>
### type="password"
When the type attribute has
a value of password it creates
a text box that acts just like a
single-line text input, except
the characters are blocked out.
They are hidden in this way so
that if someone is looking over
the user's shoulder, they cannot
see sensitive data such as
passwords.
### name
The name attribute indicates
the name of the password input,
which is sent to the server with
the password the user enters.
### size, maxlength
It can also carry the size and
maxlength attributes like the
the single-line text input.


![](https://www.wikihow.com/images/thumb/d/d7/Create-a-Password-Box-in-HTML-Step-2.jpg/v4-460px-Create-a-Password-Box-in-HTML-Step-2.jpg.webp)

# Text Area
## <-textarea>
The <-textarea> element
is used to create a mutli-line
text input. Unlike other input
elements this is not an empty
element. It should therefore have
an opening and a closing tag.
Any text that appears between
the opening <-textarea> and
closing <-/textarea> tags will
appear in the text box when the
page loads.
If the user does not delete any
text between these tags, this
message will get sent to the
server along with whatever the
user has typed. (Some sites
use JavaScript to clear this
information when the user clicks
in the text area.)



![](https://i.ytimg.com/vi/gRrRwc2_Lu8/maxresdefault.jpg)



# HTML5: Form Validation
You have probably seen forms
on the web that give users
messages if the form control has
not been filled in correctly; this is
known as form validation.
Traditionally, form validation
has been performed using
JavaScript (which is beyond the
scope of this book). But HTML5
is introducing validation and
leaving the work to the browser.
Validation helps ensure the
user enters information in a
form that the server will be able
to understand when the form
is submitted. Validating the
contents of the form before it is


to learn more about it open linik

[Forms](https://wtf.tw/ref/duckett.pdf)


# Lists, Tables & Forms
## Bullet Point Styles
### list-style-type
The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker).
It can be used on rules that
apply to the <-ol>, <-ul>, and <-li>
elements.



![](https://www.oreilly.com/library/view/html-css/9781118206911/images/ch014-Uf002.jpg)


# Images for Bullets
## list-style-image
You can specify an image to act
as a bullet point using the
list-style-image property.
The value starts with the letters
url and is followed by a pair
of parentheses. Inside the
parentheses, the path to the
image is given inside double
quotes.
This property can be used on
rules that apply to the <-ul> and
<-li> elements.
The example on this page also
shows the use of the margin
property to increase the vertical
gap between each item in the
list.


![](https://elextutorial.com/wp-content/uploads/2019/02/HTML-Unordered-List-HTML-ul.jpg)


# Positioning the Marker
## list-style-position
Lists are indented into the page
by default and the list-styleposition property indicates
whether the marker should
appear on the inside or the
outside of the box containing the
main points.
This property can take one of
two values:
# outside
The marker sits to the left of the
block of text. (This is the default
behaviour if this property is not
used.)
# inside
The marker sits inside the box of
text (which is indented).
In the example shown, the width
of the list has been limited to 150
pixels. This ensures that the text
wraps onto a new line so you can
see how the value of inside sits
the bullet inside the first line of
text.


![](https://t4tutorials.com/wp-content/uploads/2019/03/Position-The-List-Item-Marker-in-HTML-and-CSS.png)


# Border on Empty Cells
## empty-cells
If you have empty cells in
your table, then you can use
the empty-cells property to
specify whether or not their
borders should be shown.
Since browsers treat empty cells
in different ways, if you want to
explicitly show or hide borders
on any empty cells then you
should use this property.
It can take one of three values:
# show
This shows the borders of any
empty cells.
# hide
This hides the borders of any
empty cells.
# inherit
If you have one table nested
inside another, the inherit
value instructs the table cells to
obey the rules of the containing
table.


![](https://i.stack.imgur.com/TcV0P.png)

# Aligning Form Controls: Problem
Labels for form elements are
often different lengths, which
means that the form controls will
not appear in a straight line. This
is demonstrated in the example
on the right (without CSS applied
to the form controls).
In this form, each topic we ask
the user about is placed inside
a <-div> element to ensure that
each question appears on a new
line. It is easier for users to fill in
a form if the form controls are
aligned in a straight vertical line.
The CSS on the opposite page
addresses this.
If you look at where we ask
users their gender, the two
radio buttons each have their
own <-label> (one saying male
and another saying female). A
<-span> element has been added
to the title which will help align
these controls


to learn more  about it open linik

[Lists, Tables & Forms](https://wtf.tw/ref/duckett.pdf)



# Events
## What is event object in JavaScript?
When a W3C event listener's event occurs and it calls its associated function, it also passes a single argument to the function—a reference to the event object. The event object contains a number of properties that describe the event that occurred.


![](https://miro.medium.com/max/572/1*1zNMKZB4Tuoy68x9MoCl8A.png)


# What are the 8 types of JavaScript events?
+ User Interface events. These occur as the result of any interaction with the browser window rather than the HTML page.
+ Focus and blur events.
+ Mouse events.
+ Keyboard events.
+ Form events. ...
+ Mutation events and observers.
+ HTML5 events.
+ CSS events.


![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/JavaScript-Event-Types-1200x900.jpg)


# How do you create an event object?
Raising a custom event is simple; we pass the name, details and options to a new CustomEvent object: var event = new CustomEvent( "newMessage", { detail: { message: "Hello World!", time: new Date(), }, bubbles: true, cancelable: true } ); In this example, “newMessage” is the custom event type


# Event reference
Events are fired to notify code of "interesting changes" that may affect code execution. These can arise from user interactions such as using a mouse or resizing a window, changes in the state of the underlying environment (e.g. low battery or media events from the operating system), and other causes.

Each event is represented by an object that is based on the Event interface, and may have additional custom fields and/or functions to provide information about what happened. The documentation for every event has a table (near the top) that includes a link to the associated event interface, and other relevant information. A full list of the different event types is given in Event > Interfaces based on Event.

This topic provides an index to the main sorts of events you might be interested in (animation, clipboard, workers etc.) along with the main classes that implement those sorts of events. At the end is a flat list of all documented events.



# Introduction to events

Events are actions or occurrences that happen in the system you are programming, which the system tells you about so you can respond to them in some way if desired. For example, if the user selects a button on a webpage, you might want to respond to that action by displaying an information box. In this article, we discuss some important concepts surrounding events, and look at how they work in browsers. This won't be an exhaustive study; just what you need to know at this stage.


# User Interface Events
JavaScript within the browser is event driven, meaning that JavaScript responds to interactions by generating events, and expects a program to listen to interesting events. There are two types of events:

User events (such as "click" mouse events) are propagated from the DOM to the Maps JavaScript API. These events are separate and distinct from standard DOM events.
MVC state change notifications reflect changes in Maps JavaScript API objects and are named using a property_changed convention.
Each Maps JavaScript API object exports a number of named events. Programs interested in certain events will register JavaScript event listeners for those events and execute code when those events are received by calling addListener() to register event handlers on the object.

The below sample will show you what events are triggered by the google.maps.Map as you interact with the map


for more details please join link

[Event](https://www.w3schools.com/js/js_events.asp)