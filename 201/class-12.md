# Class 12 reading notes

## From the article on the Chart.js API

<https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/>

* Charts are better for displaying data visually than tables
* Charts won't get used as layout tools
* Charts are easier to look at and convey data quickly

## From The Articles on the Canvas API

Basic Usage <https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage>

* At first sight a \<canvas> element looks like an \<img> element without *src* and *alt* attributes
  * A \<canvas> element has 2 optional elements - *width* and *height* - can be set using DOM properties
* When no *width* and *height* properties are specified, the canvas will intially be 300px wide and 150px high. Element can be sized by CSS, but during rendering image can appear distorted if CSS sizing doesn't respect the ratio of the initial canvas.
* You should always provide fallback content to be displayed on older browsers that don't support the content.
* A \<canvas> element REQUIRES a closing tag. If not present, the rest of the document will be considered the fallback content and won't be displayed.

Drawing shapes with Canvas <https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes>

All elements are placed relative to the origin of the grid

\<canvas> only supports 2 primitive shapes: rectangles and paths. All other shapes must be created by combining one or more paths.

Three functions that draw rectangles:

* fillRect(x, y, width, height) - draws a filled rectangle
* strokeRect(x, y, width, height) - draws a rectangular outline
* clearRect(x, y, width, height) - clears the specified rectangular area, making it fully transparent

* Each of the above functions *x* and *y* specify the top-left corner of each rectangle

A path is a list of points, connected by segments of lines that can be of different shapes - curved or not - of different width and of different color.

* A path - or subpath - can be closed.
* To make shapes using paths, there are extra steps:
  * Create the path
  * Use drawing commands to draw into the path
  * Once path has been created, you can stroke or fill the path to render it.

Functions to perform the above steps:

* beginPath() - creates a new path. Future drawing commands are directed into the path and used to build the path up.
* closePath() - adds a straight line to the path, going to the start of the current sub-path.
* stroke() - draws the shape by stroking its outline
* fill() - draws a solid shape by filling in the path's content area

When you call *fill()* any open shapes are closed automatically so you don't have to call *closePath()* - this is NOT the case when you call *stroke()*.

Applying styles and colors <https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors>

If we want to apply colors to a shape there are 2 important properties we can use: *fillStyle* and *strokeStyle*

* *fillStyle = color* - sets the style used when filling shapes
* *strokeStyle = color* - sets the style for the shapes' outlines

* *color* is a string representing a CSS \<color>, a gradient object, or a pattern object. By default, stroke and fill color are set to black (CSS color value #000000).

* When you set the *strokeStyle* and/or *fillStyle* property, the new value becomes the default for all shapes. Must be reassigned each time you want different colors.

We can also draw semi-transparent (translucent) shapes by setting the *globalAlpha* property, or by assigning a semi-transparent color to the stroke and/or fill style.

* *globalAlpha = transparencyValue* - applies the specified transparency value to all future shapes drawn on the canvas. Value must be between 0.0 (fully transparent) to 1.0 (fully opaque) - value is 1.0 by default.

LINE STYLES

There are several properties that allow us to style lines

* lineWidth = value - sets width of lines drawn in future
* lineCap = type - sets appearance of the ends of lines (butt, round, square)
* lineJoin = type - sets appearance of "corners" where lines meet (round, bevel, miter)
* miterLimit = value - establishes a limit on the miter when 2 lines join at a sharp angle, let you control how thick the junction becomes.
* getLineDash() - returns the current line dash pattern array containing an even number of non-negative numbers
* setLineDash(segments) - sets the current line dash pattern
* lineDashOffset = value - specifies where to start a dash array on a line

Drawing text <https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text>

The canvas rendering context provides 2 methods to render text:

* fillText(text, x, y [, maxWidth]) - fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

* strokeText(text, x, y [, maxWidth]) - strokes a given text at the given (x,y) position. Optionally with a maximum with to draw.

More properties to adjust the way text gets displayed on the canvas:

* font = value - current text style being used when drawing text. Default is 10px sans-serif.
* textAlign = value - possible values: start, end, left, right, center. Default value is *start*.
* textBaseline = value - baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. Default value is *alphabetic*.
* direction = value - Directionality. Possible values: ltr, rtl, inherit. Default value is *inherit*.
