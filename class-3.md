# Ordered Lists

The HTML ol tag is used for ordered list. We can use ordered list to represent items either in numerical order format or alphabetical order format, or any format where an order is emphasized



![](https://i1.wp.com/blog.thejaytray.com/wp-content/uploads/2015/04/007-Music-HTML-UnOrdered-List-Example.png)

## <-ol->
The ordered list is created with
the <-ol> element.
# <-li>
Each item in the list is placed
between an opening <-li> tag
and a closing <-/li> tag. (The li
stands for list item.)



# Unordered Lists
An unordered list typically is a bulleted list of items. HTML 3.0 gives you the ability to customise the bullets, to do without bullets and to wrap list items horizontally or vertically for multicolumn lists

# <-ul>
The unordered list is created
with the <-ul> element.
# <-li>
Each item in the list is placed
between an opening <-li> tag
and a closing </-li> tag. (The li
stands for list item.)



![](https://i.ytimg.com/vi/G56inbH_a48/maxresdefault.jpg)

---------------------------------------
---------------------------------------

# Definition Lists

A definition list is a list of terms and corresponding definitions. Definition lists are typically formatted with the term on the left with the definition following on the right or on the next line. The definition text is typically indented with respect to the term

 # <-dl>
 The definition list is created with
 the <-dl> element and usually
 consists of a series of terms and
 their definitions.
 Inside the <-dl> element you will
 usually see pairs of <-dt> and
<-dd> elements.

# <-dt>
This is used to contain the term
being defined (the definition
term).

# <-dd>
This is used to contain the
definition.
Sometimes you might see a list
where there are two terms used
for the same definition or two
different definitions for the same
term.



![](https://www.wikihow.com/images/thumb/c/c7/Define-a-Definition-List-in-HTML-Step-11.jpg/v4-460px-Define-a-Definition-List-in-HTML-Step-11.jpg.webp)






#
# Boxes
## Box Dimensions width, height
The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems. Traditionally, pixels have
been the most popular method
because they allow designers to
accurately control their size.
When you use percentages,
the size of the box is relative to
the size of the browser window
or, if the box is encased within
another box, it is a percentage of
the size of the containing box.



![](https://s3.amazonaws.com/media.skillcrush.com/skillcrush/wp-content/uploads/2018/03/boxmodel.png)




## Limiting Width min-width, max-width
These are very helpful properties
to ensure that the content of
pages are legible (especially on
the smaller screens of handheld
devices). For example, you can
use the max-width property to
ensure that lines of text do not
appear too wide within a big
browser window and you can
use the min-width property
to make sure that they do not
appear too narrow.
You may find it helpful to try this
example out in your browser so
that you can see what happens
when you increase or decrease
the size of the browser window



![](https://slidetodoc.com/presentation_image_h/8aacec8cb58ac300d64e39bdc731faaa/image-5.jpg)




## Limiting Height min-height, max-height
In the same way that you might
want to limit the width of a box
on a page, you may also want
to limit the height of it. This is
achieved using the min-height
and max-height properties



![](https://i0.wp.com/css-tricks.com/wp-content/uploads/2020/05/Screen-Shot-2020-05-25-at-12.24.35-PM.png?resize=659%2C371&ssl=1)




## Border, Margin & Padding
### Border
Every box has a border (even if
it is not visible or is specified to
be 0 pixels wide). The border
separates the edge of one box
from another.



![](https://www.dummies.com/wp-content/uploads/412492.image1.jpg)


### Margin
Margins sit outside the edge
of the border. You can set the
width of a margin to create a
gap between the borders of two
adjacent boxes.




![](https://i.pinimg.com/originals/61/f2/71/61f271bb01d3b693943cae6ca63ec311.png)




### Padding
Padding is the space between
the border of a box and any
content contained within it.
Adding padding can increase the
readability of its contents.








# LASHCARDS IN CHAPTER 2: BASIC JAVASCRIPT INSTRUCTIONS DECK (20)
1. Statements
An individual instruction or step in javascript. Ends with a semi colon

var today = new Date();

2. Comments
Used to explain code. You can have multi line using syntax /* */ or single line using // syntax . Any script surrounded by a comment is not processed by the js interpreter

3. Is Javascript a case sensitive language?
Yes. hournow and hourNow would be treated as two different items

4. code block
lines of code surrounded by curly braces { } do not end in a semi colon

5. Variable
variables are used to store bits of information. If you need to reuse a piece of information you're best to store it in a variable. Programmers say you declare a variable. You can then assign it a value. Variables stand in for a value, so rather than saying the specific number it represents (which may change), its use whatever is stored in this item instead

var dinosaur = "Spinosaurus";

6. This is the assignment operator. it assigns a value to a variable.

7. undefined
Until a variable has a value its undefined

8. Data types
Javascript variables can have a range of types.
numeric (e.g. 2, 0.75)
String ("Used for text)
Boolean (results in a true or false value)

There's also arrays, objects, undefined and null

9. Quote marks
Used to mark out strings. You can use single or double but they must match i.e. don't start with string ' and end with "

10.  escaping quotes
Used when you want to show quote marks inside a string.

You can either use a backslash before a quote mark or Start the string with double quotes and then use single quotes inside the string

11. Booleans are useful...
+  When a value can only be true or false

+ When code can take more than a single path (allows us to test if a condition/s are true or false)

12. Rules for naming variables
+ must begin with a letter, dollar sign or underscore
+ names can contain letters, numbers, $ or an underscore
+ You cannot use keywords/reserved words
+ case sensitive
+ use a name that describes the info that the variable stores
+ camelcase

13. Array
Arrays store a list of values or related values. The values are indexed by a number starting at 0.

Using an array is useful instead of creating individual variables when you are unsure of the number of items

var colours = ['white', 'black', 'red'];

14. array literal syntax vs array constructor sytax
literal:
var colours = ['white', 'black', 'red'];

constructor:
var colours = new Array ('white', 'black', 'red');

15. Access values in an array
by index number

var colours = ['white', 'black', 'red'];

colours[2];

by item

var colours = ['white', 'black', 'red'];

colours.item(1);

16. What does array.length do?
Returns how many items are in the array

17. What is an expression?
An expression evaluates to a single value.

we can either assign a value

or

write an expression that uses two or more values to return a single value

18. What is an operator
It's a tool that allows us to combine multiple values into a single value.

Assignment, Aritmatic, String (+ this combines strings and numbers together concatenates)

19. What is the % modulus operator
When doing division it returns the remainder



![](https://mozilla.github.io/webmaker-curriculum/QuackingJavascript/images/thimble_simple.png)



-------------------------
-------------------------


# Decisions and Loops
## what is the switch statements?

In computer programming languages, a switch statement is a type of selection control mechanism used to allow the value of a variable or expression to change the control flow of program execution via search and map



![](https://www.codegrepper.com/codeimages/javascript-switch-case-range.png)





# Does JavaScript have a switch statement?
In addition to if...else , JavaScript has a feature known as a switch statement. switch is a type of conditional statement that will evaluate an expression against multiple possible cases and execute one or more blocks of code based on matching cases







# What is switch statement example?
A general syntax of how switch-case is implemented in a 'C' program is as follows: switch( expression ) { case value-1: Block-1; Break; case value-2: Block-2; Break; case value-n: Block-n; Break; default: Block-1; Break; } Statement-x; The expression can be integer expression or a character expression




![](https://www.theengineeringprojects.com/wp-content/uploads/2020/01/Switch-Statment-in-JavaScript-1.jpg)



# Is switch statement better than if else?
A switch statement is usually more efficient than a set of nested ifs. The compiler can do this because it knows that the case constants are all the same type and simply must be compared for equality with the switch expression, while in case of if expressions, the compiler has no such knowledge.









