# Class 7 reading notes

## ["Domain Modeling"](https://github.com/codefellows/domain_modeling#domain-modeling)

* When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
* Model its attributes with a constructor function that defines and initializes properties.
* Model its behaviors with small methods that focus on doing one job well.
* Create instances using the "new" keyword followed by a call to a constructor function.
* Store the newly created object in a variable so you can access its properties and methods from outside.
* Use the "this" variable within methods so you can access the object's properties and methods from inside

## From the Duckett HTML & CSS Book

## Chapter 6: "Tables" (pg 126-145)

Basic Table Structure:

* `<table>` - creates table element. Content is written out row by row.
* `<tr>` - stands for "table row", closed with `</tr>` at end of row
* `<td>` - stands for "table data", use `</td>` at end of each cell

Some browsers automatically draw lines around the table and/or individual cells. Control this with CSS.

* `<th>` - table heading for either column or row

There are 3 elements that help distinguis between main content of table and first and last rows.

* `<thead>` - headings should be inside here, close with \</thead>
* `<tbody>` - all body content inside here, close with `</tbody>`
* `<tfoot>` - footer inside here, close with `</tfoot>`

^^ These aren't treated differently from other elements, but CSS styles are used to change appearance

## From the Duckett JS & JQuery Book

## Chapter 3: "Functions, Methods, and Objects" (pg 106-144)

In JS, to organize your data you can use an array or object to group a set of related values.

Arrays are actually a special type of object. They hold a related set of key/value pairs (like all objects), but the key for each value is its index number.

You can combine arrays and objects to create complex data structures: Arrays can store a series of objects (and remember their order). Objects can also hold arrays (as values of their properties).

Browsers come with a set of built-in objects that represent things like the browser window and the current webpage shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

* First thing you need to do is get to know what tools are available. Imagine your new "toolkit" has 3 compartments:
  * Browser Object Model - contains objects that represent current browser window or tab
  * Document Object Model - uses objects to create a representation of current page
  * Global JavaScript Objects - represent things the JavaScript language needs to create a model of.
