# Class 11 reading notes

## From the Duckett HTML & CSS Book

### Chapter 9 pages 201-206 - SKIM ONLY

* Flash is no longer supported by many browsers
* Flash is a very popular technology used to add animations, video and audio to websites

### Chapter 16: "Images" (pg 406-427)

SIZE AND ALIGNMENT

* Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.

* A lot of sites use the same sized image across many of their pages.

* Whenever you use consistently sized images across a site, you can use CSS to control the dimensions of the images instead of putting the dimensions in the HTML.
  * First, determine sizes of images commonly used throughout the site then give each size a name (small, medium, large)
  * Where the `<img>` elements appear in the HTML, use these names as values for the *class* attribute
  * In CSS add selectors for each of the class names, then use CSS *width* and *height* properties to control the image dimensions

* Rather than using the `<img>` element's *align* attribute, authors are increasingly using *float* property to align images.
  * *Float* property is added to the class that was created to represent the size of the image (such as the *small* class)
  * New classes are created with names such as *align-left* or *align-right* to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.

* By default, images are inline elements.
* In order to center an image, it should be turned into a block-level element using the *display* property with a value of *block*
* Once it has been made into a block-level element, there are 2 ways to horizontally center it:
  * On the containing element, use *text-align* property with a value of *center*
  * On the image itself, you can use *margin* property and set the values of the left and right margins to *auto*.
* You can also specify class names that allow any element to be centered, in the same way that you can for the dimensions or alignment of images.
* The technique for specifying image size and alignment can also be used with the HTML5 *`<figure>`* element.

BACKGROUND IMAGES

* The *background-image* property allows you to place an image behind any HTML element. This could be the entire page or just part of a page. By default, a background image will repeat to fill the entire box.

* The path to the image follows the letters *url* and it is put inside parentheses and quotes.

* Background images are often the last thing to load on a page which can make the website seem slow to load.

* The *background-repeat* property can have 4 values:
  * repeat -- image is repeated horizontally AND vertically
  * repeat-x -- image is repeated horizontally only
  * repeat-y -- image is repeated vertically only
  * no-repeat -- image is only shown once
* The *background-attachment* property specifies whether a background image should stay in 1 position or move as the user scrolls. It can have one of two values:
  * fixed -- image stays in same position on page
  * scroll -- image moves as user scrolls
* When an image is not being repeated you can use *background-position* property to specify where in the browser window the image should be placed. This property usually has a pair of values. (left top, left center, left bottom, center top, center center, center bottom, right top, right center, right bottom)
  * The first represents horizontal position
  * The second represents vertical position
  * If you only specify one value, the second value will default to *center*
* You can also use a pair of pixels or percentages. These represent the distance from the top left corner of the browser window OR containing box. Top left corner is equal to 0% 0%. To center image horizontally and vertically, 50% 50% is used.

* The *background* property is shorthand for ALL the other background properties.

* Properties must be specified in the following order, but you can miss any value if you do not want to specify it:
  * background-color
  * background-image
  * background-repeat
  * background-attachment
  * background-position

IMAGE ROLLOVERS AND SPRITES

* Using CSS it is possible to create a link or a button that changes style when a user moves their mouse over it. This is achieved by setting a background image for the link/button that has 3 different styles of the same button (but only allows enough space to show one of them at a time)
* When the user moves their mouse over the element, or clicks on it, position of background image is moved to show relevant image.
* When a single image is used for several different parts of an interface, it is known as a SPRITE. You can add the logo and other interface elements, as well as buttons to the image.
* The advantage of using sprites is that the web browser only needs to request one image rather than many images, which can make the page load faster.

GRADIENTS

* CSS3 is going to introduce the ability to specify a gradient for the background of a box.

CONTRAST OF BACKGROUND IMAGES

* If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible.
* To overlay text on an image with high contrast, you can place a semi-transparent background color (or "screen") behind the text to improve legibility.

### Chapter 19: "Practical Information" (pg 476-492)

SEARCH ENGINE OPTIMIZATION (SEO)

* SEO is the practice of trying to help your site appear nearer to the top of search engine results when people look for the topics that your website covers

* Working out which terms people are likely to enter into a search engine to find your site, using these terms in the right places on your site to increase chances of search engines showing a link to your site in their results.

* SEO is often split into two areas:
  * On-page techniques
    * Methods you can use on your page to improve rating in search engines
    * There are 7 essential places where you want your keywords to appear
    * Any images have appropriat text in their *alt* attribute also helps search engines understand content of your images
  * Off-page techniques
    * Getting other sites to link to your page
    * Search engines are particularly interested in sites whose content is related to yours.
    * Search engines also look at the words between your opening and closing `<a>` tags in the link. If the text in the link contains keywords rather than just *click here* or your website address, it may be considered more relevant.
    * The words that appear in links to your site should also appear in the text of the page that the site links to.

* SEVEN KEY PLACES WHERE KEYWORDS SHOULD APPEAR
  * Page title
  * URL/Web address
  * Headings
  * Text
  * Link text
  * Image Alt text
  * Page descriptions

* Never try to fool search engines!!! They will penalize you for it. For example, never add text in the same color as the background of the page, as search engines can detect this.
* 6 STEPS TO IDENTIFY KEYWORDS AND PHRASES
  * Brainstorm
  * Organize
  * Research
  * Compare
  * Refine
  * Map

DOMAIN NAMES & HOSTING

* In order to put your site on the web you will need a domain name and web hosting.
  * Domain name is your web address.
    * There are many websites that allow you to register domain names. Usually you will have to pay an annual fee to keep that domain name.
  * Most websites live on web servers run by web hosting companies. This is usually far cheaper and more reliable than trying to run your own web servers.
    * There are lots of different types of hosting on offer. Some things to help choose which hosting company to use:
      * Disk space - total size of all the files that make up your site
      * Bandwidth - amount of data the hosting company will send to your site's visitors.
      * Backups - check whether the hosting company performs backups on your site and how often.
      * Email accounts - check the size of the mailbox you are allowed, and the number of mailboxes you can use.
      * Server-Side languages and databases - be sure to check that your hsoting company supports the technologies your software needs to run.
