# What's a Table?
A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results Grids allow us to understand
complex data by referencing
information on two axes.
Each block in the grid is referred
to as a table cell. In HTML a
table is written out row by row

## Basic Table Structure
### <-table>
The <-table> element is used
to create a table. The contents
of the table are written out row
by row.
### <-tr>
You indicate the start of each
row using the opening <-tr> tag.
(The tr stands for table row.)
It is followed by one or more
<-td> elements (one for each cell
in that row).
At the end of the row you use a
closing <-/tr> tag
### <-td>
Each cell of a table is
represented using a <-td>
element. (The td stands for
table data.)
At the end of each cell you use a
closing <-/td> tag.


![basic of table](https://www.oreilly.com/library/view/web-design-in/1565925157/tagoreillycom20070306oreillyimages157933.png)




# Table Headings
## <-th>
The <-th> element is used just
like the <-td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)
Even if a cell has no content,
you should still use a <-td> or
<-th> element to represent
the presence of an empty cell
otherwise the table will not
render correctly. (The first cell
in the first row of this example
shows an empty cell.)
Using <-th> elements for
headings helps people who
use screen readers, improves
the ability for search engines
to index your pages, and also
enables you to control the
appearance of tables better
when you start to use CSS.
You can use the scope attribute
on the <-th> element to indicate
whether it is a heading for a
column or a row. It can take the
values: row to indicate a heading
for a row or col to indicate a
heading for a column.



![table heading](https://docs.wingarc.com.au/superstar95/files/latest/66355970/66552858/1/1452471722672/Modify-Header-Footer.png)



# Long Tables
There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).
These elements help people
who use screen readers and also
allow you to style these sections
in a different manner than the
rest of the table (as you will see
when you learn about CSS).
### <-thead>
The headings of the table should
sit inside the <-thead> element.

### <-tbody>
The body should sit inside the
<-tbody> element.

### <-tfoot>
The footer belongs inside the
<-tfoot> element.


![long table](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ20kOQ00kwUoplmhZoEpe5txsOzxW60gfRaA&usqp=CAU)



for more details please join the link 
[table](https://wtf.tw/ref/duckett.pdf)




---------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------

# Functions, Methods, and Objects.
## What are methods and objects?
### Object-Oriented Terminology

object: an object is an element (or instance) of a class; objects have the behaviors of their class. ... a method is an action which an object is able to perform. sending a message. sending a message to an object means asking the object to execute or invoke one of its methods.


## How are functions objects?
Values can be passed to a function, and the function will return a value. In JavaScript, functions are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called. In brief, they are Function objects

## Are Java functions objects?
A functor is an object that's a function. Java doesn't have them, because functions aren't first-class objects in Java


![](https://i.ytimg.com/vi/yrIbbKuSqK8/maxresdefault.jpg)



#### In JavaScript, functions are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called. In brief, they are Function objects. For more examples and explanations, see also the JavaScript guide about functions


# Functions
Generally speaking, a function is a "subprogram" that can be called by code external (or internal in the case of recursion) to the function. Like the program itself, a function is composed of a sequence of statements called the function body. Values can be passed to a function, and the function will return a value.

In JavaScript, functions are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called. In brief, they are Function objects.

For more examples and explanations, see also the JavaScript guide about functions.

# Description
Every function in JavaScript is a Function object. See Function for information on properties and methods of Function objects.

To return a value other than the default, a function must have a return statement that specifies the value to return. A function without a return statement will return a default value. In the case of a constructor called with the new keyword, the default value is the value of its this parameter. For all other functions, the default return value is undefined.

The parameters of a function call are the function's arguments. Arguments are passed to functions by value. If the function changes the value of an argument, this change is not reflected globally or in the calling function. However, object references are values, too, and they are special: if the function changes the referred object's properties, that change is visible outside the function



for more details please join the link 

[Functions, Methods, and Objects.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions)





