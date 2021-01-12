# Class 2 reading notes

## From the Duckett HTML Book

### Chapter 2: "Text" (pg 40-61)

There are 2 kinds of markup:

* structural markup: elements you can use to describe both headings AND paragraphs
* semantic markup: provides extra info for browser such as where emphasis is placed in a sentence, if something is a quote, acronyms, etc\.

HTML has 6 "levels" of headings

By default a browser will show space between new paragraphs

* Superscript: use \<sup>\</sup> element - for date suffixes, mathematical concepts, etc\.
* Subscript: use \<sub>\</sub> element - for foot notes, chemical formulas, etc\.

WHITE SPACE COLLAPSING: two or more spaces next to each other or a line break, browser treats it as a single space.

* Webpage authors take advantage of this by using it when indenting code for easier readability.

To create a line break INSIDE a paragraph, use \<br />

To insert a horizontal line between paragraphs, use \<hr />

* Both of the above are considered EMPTY ELEMENTS. They only have 1 tag and a space and forward slash before the closing bracket\.

SEMANTIC MARKUP - \<em> and \<blockquote> are NOT for changing the way text looks. They are used for sreen readers, search engines, etc to use as extra information.
*example: screen reader voice adds emphasis to words inside \<em> elements

TO MARKUP QUOTATIONS - there are 2 ways:

* \<blockquote>\</blockquote> - for longer quotes that are a whole paragraph. \<p> element is still used inside \<blockquote> element. Browsers tend to indent these \<blockquote> elements, but don't use JUSt to indent. Use CSS for this\.

* \<q>\</q> - for shorter quotes, element is used inside the \<p> element.

Both above elements may use cite attribution to indicate where quote is from: \<blockquote cite="URL">\</blockquote>

\<abbr> - for abbreviations or acronyms

* \<p>\<abbr title="Professor">Prof\</abbr>\</p>

\<cite>Source\</cite>  to indicate where citation is from

* in HTML5 \<cite> should not be used for a person's name
* browser will render content of \<cite> element in italics

\<dfn> - used for the first time you explain some new terminology. Stands for "defining instance of" - some browsers show the content of a \<dfn> element in italics, Safari & Chrome do not

### Chapter 10: "Introducing CSS" (pg 226-245)

## From the Duckett JS book

### Chapter 2 "Basic JavaScript Instructions" (pg 53-84)

### Chapter 4 "Decisions and Loops" (pg 145-162) *only up to the section on switch statements*

## Additional Resources

<https://chris.beams.io/posts/git-commit/>
