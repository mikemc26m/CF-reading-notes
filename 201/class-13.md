# Class 13 reading notes

## From "The Past, Present and Future of Local Storage for Web Applications"

<http://diveinto.html5doctor.com/storage.html>

Cookies were invented early in web history but have 3 major downsides:

* Cookies are included w/ every HTTP request, slowing down web application by transmitting same data over and over
* Sending data unencrypted over the internet
* Limited to about 4KB of data - enough to slow down your application but not enough to be terribly useful

HTML5 Storage - a specification named Web Storage - which was at one time part of HTML5 specification proper, but was split out into its own specification.
  
* Also referred to as "local storage" or "DOM Storage"

What IS HTML5 Storage? A way for web pages to store named key/value pairs locally, within the client web browser.

* The data persists even after you navigate away from the site, close browser tab, exit browser, etc.
* Data is never transmitted to the remote web server

HTML5 Storage is based on named key/value pairs. You store data based on a name key, you can retrieve that data with the same key. The named key is a STRING.

* If you are storing and retrieving anything OTHER than strings, you will need to use functions to coerce your retrieved data into the expected JS datatype.

You can keep track programmatically when the storage area changes by trapping the ````storage```` event.

* The ````storage```` event is fired on the ````window```` object whenever ````setItem()````, ````removeItem()````, or ````clear()```` is called and *actually changes something*.
  * If you set an itme to its existing value or call ````clear()```` when there are no named keys, the ````storage```` event will not fire, because nothing actually changed in the storage area.
