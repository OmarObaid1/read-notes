# Tutorial: Intro to React
## Before We Start the Tutorial
We will build a small game during this tutorial. You might be tempted to skip it because you’re not building games — but give it a chance. The techniques you’ll learn in the tutorial are fundamental to building any React app, and mastering it will give you a deep understanding of React.

# What Are We Building?
In this tutorial, we’ll show how to build an interactive tic-tac-toe game with React.

You can see what we’ll be building here: Final Result. If the code doesn’t make sense to you, or if you are unfamiliar with the code’s syntax, don’t worry! The goal of this tutorial is to help you understand React and its syntax.

We recommend that you check out the tic-tac-toe game before continuing with the tutorial. One of the features that you’ll notice is that there is a numbered list to the right of the game’s board. This list gives you a history of all of the moves that have occurred in the game, and it is updated as the game progresses.

# What Is React?
React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

React has a few different kinds of components, but we’ll start with React.Component subclasses:

![](https://s3.amazonaws.com/media.skillcrush.com/skillcrush/wp-content/uploads/2019/05/Screen-Shot-2019-05-14-at-10.33.05-AM.png.webp)


# Passing Data Through Props
To get our feet wet, let’s try passing some data from our Board component to our Square component.

We strongly recommend typing code by hand as you’re working through the tutorial and not using copy/paste. This will help you develop muscle memory and a stronger understanding.

In Board’s renderSquare method, change the code to pass a prop called value to the Square:
![](https://tech4grasp.com/wp-content/uploads/2019/08/functional-children.png)


## Wrapping Up
Congratulations! You’ve created a tic-tac-toe game that:

Lets you play tic-tac-toe,
Indicates when a player has won the game,
Stores a game’s history as a game progresses,
Allows players to review a game’s history and see previous versions of a game’s board.
Nice work! We hope you now feel like you have a decent grasp of how React works.

Check out the final result here: Final Result.

If you have extra time or want to practice your new React skills, here are some ideas for improvements that you could make to the tic-tac-toe game which are listed in order of increasing difficulty:

1. Display the location for each move in the format (col, row) in the move history list.
2. Bold the currently selected item in the move list.
3. Rewrite Board to use two loops to make the squares instead of hardcoding them.
4. Add a toggle button that lets you sort the moves in either ascending or descending order.
5. When someone wins, highlight the three squares that caused the win.
6. When no one wins, display a message about the result being a draw.
--------------------------------------
# Hello World
![](https://4cawmi2va33i3w6dek1d7y1m-wpengine.netdna-ssl.com/wp-content/uploads/2016/03/2_2_HTML-and-CSS-Basics.png)

## How to Read This Guide
In this guide, we will examine the building blocks of React apps: elements and components. Once you master them, you can create complex apps from small reusable pieces.

This is the first chapter in a step-by-step guide about main React concepts. You can find a list of all its chapters in the navigation sidebar. If you’re reading this from a mobile device, you can access the navigation by pressing the button in the bottom right corner of your screen.


------------------------------------------------
# Introducing JSX
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRQuxXKSAMQ3X8SLOlrfG2XwFnmCcaQlprIqQ&usqp=CAU)
This funny tag syntax is neither a string nor HTML.

It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

JSX produces React “elements”. We will explore rendering them to the DOM in the next section. Below, you can find the basics of JSX necessary to get you started.

## Why JSX?
React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

With that out of the way, let’s get started!

## Embedding Expressions in JSX
In the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:
![](https://vegibit.com/wp-content/uploads/2019/03/react-fragment-removes-extra-divs.png)

---------------------------------------------
# Rendering Elements
![](https://tutorialspoint.dev/image/RenderingSimpleElement_ReactJS-1.jpg)

Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

# Rendering an Element into the DOM
![](https://cdn-media-1.freecodecamp.org/images/1*mXjNHOx9bbQ5D4sSUAX2Lg.png)

We call this a “root” DOM node because everything inside it will be managed by React DOM.

Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

## Updating the Rendered Element
React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render().

Consider this ticking clock example:
![](https://1.bp.blogspot.com/-nW9l_3vjIkM/XdI0t-fCk3I/AAAAAAAAVfI/VohDaa4ixjM23AhOllLyLiVZ7zxiM4rIwCLcBGAsYHQ/s1600/react-meta-tags-with-dynamic-value-in-react-js.png)



