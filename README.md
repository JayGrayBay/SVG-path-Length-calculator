# SVG Path Length Calculator

This simple project allows you to calculate the lengths of SVG paths in a given SVG image. It uses JavaScript to calculate and log the lengths in the console. 

## Setup

1. Clone this repository or download the HTML file.
2. Replace the SVG paths in the HTML file with your own SVG paths. Make sure to assign each path an `id`.
3. Open the HTML file in a web browser. The lengths of the paths are printed in the JavaScript console.

## Customization

To customize this project for your own needs, modify the SVG paths in the HTML file.

Here is an example of an SVG path:

<path id="your-path-id" d="M10 10 H 90 V 90 H 10 Z" fill="transparent" stroke="black"/>

Replace "your-path-id" with a unique ID for this path.
  
Replace the d attribute with the definition of your path. This is a mini language that defines the shape of the path. For example, M10 10 H 90 V 90 H 10 Z draws a square.


If you want to do something with the lengths other than logging them to the console, modify the JavaScript code in the window.onload function.

javascript

window.onload = function() {
  var paths = document.querySelectorAll('.anim2 path');

  paths.forEach(path => {
    console.log(path.id, path.getTotalLength());
    // Add your code here. For example, you might want to display the lengths on the page.
  });
}




