# Class 3 reading notes

## From the Duckett HTML Book

### Chapter 3: "Lists" (pg 62-73)

* Definition lists are created with \<dl> element, inside are \<dt> and \<dd> elements for definition term and definition, respectively.

* Nested lists are created by putting another \<ul> inside a list. Browsers display nested lists indented further than parent lists, and default browser rules usually change bullet style too.

### Chapter 13: "Boxes" (pg 300-329)

* By default a box is sized big enough to hold its contents.

* Most popular ways to specify box size are px, percentages, or em. Pixels are popular for accurate control.

* When using percentages, size of the box is relative to size of browser window - OR - if it's encased within another box, it's the percentage of the size of that box.

* Using em measurements is based on the size of the text within the box

* Min-width and max-width properties specify smallest and maximum widths boxes can be

* Overflow is used if the box is not big enough to hold the content. Hidden OR scroll.

* EVERY BOX HAS 3 AVAILABLE PROPERTIES TO CONTROL APPEARANCE:
  * Border - seperates edge of one box from another
  * Margin - sits outside the edge of the border
  * Padding - space between border of the box and any content inside the box

* The border-width property controls width of border using pixels or values: thin/medium/thick - You CANNOT use percentages.

* You can control individual sides of border:

  * border-top-width
  * border-right-width
  * border-bottom-width
  * border-left-width
  * Specify all 4 values in  property. Example - border-width: 2px 1px 1px 2px; (clockwise top, right, bottom, left)
* The border-style property values:

  * solid
  * dotted
  * dashed
  * double
  * groove
  * ridge
  * inset
  * outset
  * hidden/none

* BORDER SHORTHAND - allows you to set width, style and color of a border in one property - values coded in that order
  * Example - p \{border: 3px dotted #0088dd;\}

* Centering content
* Change inline/block/inline-block/none
* Hiding boxes - hidden or visible
* Border images
* Box shadow
* Rounded corners - in CSS3
  * border-radius indicates size of the radius in pixels
  * border-top-right/left-radius
  * border-bottom-right/left-radius
  
## From the Duckett JS book

### Review Chapter 2 pg 70-73: ARRAYS

* Array doesn't just store 1 variable, it stores a list of variables
* Array should be used whenever the list or set of values are related to each other.
* Arrays are especially helpful when you don't know how many items the list will contain.
* Arrays do not need to specify how many values it will hold.
* Values in an array are separated by commas.
  * Array literal - created with square brackets
  * Array constructor - created with parenthesis
* Each item in an array is given a number called an index
  * INDEX ALWAYS STARTS AT 0

### Chapter 4: "Decisions and Loops" - from Switch Statements on (pg 162-182)

IF...ELSE STATEMENTS

* if... is the code used to determine if a condition evaluates to true, Else is the code used after a condition evaluates to false

SWITCH STATEMENTS - an alternative to if...else statements

* Indicates a possible value for this variable and the code that should run if the variable matches that value.