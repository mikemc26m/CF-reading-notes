# Class 8 reading notes

## From the Duckett HTML & CSS Book

### Chapter 15: "Layout" (repeat of Class 4 reading (pg 358-404)

CSS PROPERTY: POSITION

example:

```element { position: static/relative/absolute/fixed }```

* Normal Flow - default behavior
* Relative Positioning - shifts element to top, right, bottom, or left of where it WOULD have been
* Absolute Positioning - takes it out of flow, doesn't affect surrounding elements. Moves as user scrolls up and down the page.
  * Fixed Positioning - form of absolute positioning - positions element in relation to browser window AS OPPOSED TO containing element
* Floating Elements - take element out of normal flow, position to far left or right of container. Floated element becomes block-level around which, other content can flow.

Z INDEX PROPERTY - control which box is on top of overlapping boxes caused by removing elements from normal flow.

CLEARING FLOATS

"Clear" property allows you to say that no element within the same containing element should touch the left or right hand sides of a box. (left, right, both, neither)
