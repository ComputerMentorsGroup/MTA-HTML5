# Lesson 7

In Lesson 7 we explore the differences between drawing with Canvas and SVG web technologies.

### Instructions
1. Visit www.codepen.io
2. Click Create - New Pen
3. Please note, this will be a temporary design unless you choose to make an account on Codepen.io
4. Using the information provided, try to draw a picture using SVG and Canvas - this could be your logo!


**Criteria for the Lesson 7 webpage:**
* Must use SVG
* Must use Canvas
* Implement a design into your own website 


## Drawing a Red Square in Canvas

In the HTML side of your codepen, put:
```HTML5
<canvas id="myCanvas" width="800" height="800"></canvas>
```

In the JavaScript side of your codepen, put:
```Javascript
var canvas = document.getElementById('myCanvas');
var context = canvas.getContext('2d');
context.fillStyle = '#c00';
context.fillRect(10, 10, 100, 100);
```


## Drawing a Red Square in SVG

In the HTML side only, put:
```HTML5
<svg xmlns="http://www.w3.org/2000/svg" viewbox="0 0 600 600">
  <desc>Red rectangle shape</desc>
  <rect x="10" y="10" width="100" height="100" fill="#c00"  />  
</svg>
```


## What's the difference between SVG and Canvas?

* SVG is great for two dimensional graphics.
* SVG uses XML to create vector based graphics - meaning the images are scalable without deteriorating the quality
* SVG graphics are great for creating games since they are interactive, dynamic, and can be animated using scripts
* You may use programs like Inkscape.com or Adobe Photoshop to generate SVG code for your images
* SVG graphics use **retained mode** which means you give the object some properties and the browser stores the process to create the image in its memory.
* Canvas uses **immediate mode** which means you, as a developer, need to work out the commands to draw each object to show exactly what you want.  It uses a "Fire and Forget" model, meaning it runs the commands once to display the image and is not aware of the object afterwards.
* Canvas is great for creating 3D graphics, drawing a lot of objects on a small surface, and pixel replacement in videos
* Canvas is NOT great for high quality resizing of graphics (scalability)
* Canvas requires JavaScript


# Challenge 7

A challenge relating to the original sample code should go here.

```HTML5
// Sample code should that demonstrates what should be taught in this lesson should go here
```

* CRITERIA
    * item
    * item
    * item
