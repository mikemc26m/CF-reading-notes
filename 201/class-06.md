# Class 6 reading notes

## ["Understanding The Problem Domain Is The Hardest Part Of Programming"](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

"Problem domains are like a puzzle with a blurry picture or no picture at all."

"Understanding the problem is the most critical piece to the equation."

"If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

* Make the problem domain easier
* Get better at understanding the problem domain

"You can often make the problem domain easier by cutting out cases or narrowing your focus to a particular part of the problem."

## From the Duckett JS Book

## Chapter 3: "Object Literals" (pg 100-105)

Objects group together a set of variables & functions to create a model of something you would recognize from the real world.

* In an object, VARIABLES become known as PROPERTIES
* In an object, FUNCTIONS become known as METHODS
* In an object, the NAME of functions and methods becomes known as a KEY
  * Objects cannot have 2 keys with the same name

* Value of a PROPERTY can equal a string, number, Boolean, array or even another object.
* Value of a METHOD is always a function

CREATING AN OBJECT:

LITERAL NOTATION -- Easiest and most popular way to create objects

* You can access properties or methods of an object using DOT notation

## Chapter 5: "Document Object Model (DOM)" (pg 183-242)

* DOM stands for Document Object Model.
* DOM is neither part of HTML nor JavaScript, it is a separate set of rules covering 2 major areas:
  * Making a model of the HTML page
  * Accessing and changing the HTML page

DOM is sometimes called an API (Application Programming Interface) - it lets programs and scripts talk to each other

* DOM states what your script can ask the browser about the current page, and how to tell the browser to update what is being shown to the user.

DOM Tree is a model of a webpage

* Contains four main types of nodes:
  * Document node
  * Element node
  * Attribute node
  * Text node
* Attribute nodes are NOT children of the element that carries them, they are PART of that element
* Text modes cannot have children
