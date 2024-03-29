# Color-changing-rectangle
HTML:
This is a basic HTML structure with a div element having an id of "center".
It includes links to an external CSS file (style.css) and two scripts: GSAP library and a custom JavaScript file (script.js).
CSS (style.css):
Resets default margin, padding, and sets box-sizing to border-box for all elements.
Sets the font family for the entire document.
Makes HTML and body take up the full height and width of the viewport.
Styles the #center div to be positioned at the center of the viewport with a fixed width and height, and a black border.
JavaScript (script.js):
Retrieves the #center div element from the DOM.
Adds an event listener to the #center div for the mousemove event.
Inside the event listener, it calculates the position of the mouse cursor relative to the #center div using getBoundingClientRect().
Determines whether the mouse cursor is on the left or right half of the #center div.
Uses GSAP's mapRange() method to map the mouse position to RGB color values.
Animates the background color of the #center div to change dynamically based on the mouse position.
Adds another event listener for the mouseleave event to reset the background color of the #center div when the mouse leaves the div.
GSAP (GreenSock Animation Platform):
GSAP is a powerful JavaScript library for creating high-performance animations.
It provides methods like to() for animating CSS properties.
gsap.utils.mapRange() is used to map a value from one range to another. In this case, it maps the mouse position to RGB color values.
getBoundingClientRect():
getBoundingClientRect() is a method available on DOM elements that returns the size of an element and its position relative to the viewport.
It returns a DOMRect object with properties such as top, bottom, left, right, width, and height.
In this script, getBoundingClientRect() is used to calculate the position of the mouse cursor relative to the #center div.
