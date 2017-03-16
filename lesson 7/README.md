# Lesson 7

In Lesson 7 we explore the differences between drawing with Canvas and SVG web technologies.

### Instructions
1. Visit www.codepen.io
2. Click Create - New Pen
3. Please note, this will be a temporary design unless you choose to make an account on Codepen.io
4. Using the information provided, try to draw a picture using SVG and Canvas - this could be your logo!


**Criteria for the Lesson 7 web page:**
* Must use SVG (Scalable Vector Graphics)
* Must use Canvas
* Implement a design into your own website 





# Canvas

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

## Drawing a Circle in Canvas
In the JavaScript side of your codepen, put:
```JavaScript
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(95,50,40,0,2*Math.PI);
ctx.stroke();
```

## Drawing Text in Canvas
In the JavaScript side of your codepen, put:
```JavaScript
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.fillText("Hello World",10,50);
```


## Using Gradients in Canvas
In the JavaScript side of your codepen, put:
```JavaScript
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createLinearGradient(0,0,200,0);
grd.addColorStop(0,"red");
grd.addColorStop(1,"white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10,10,150,80);
```

For the full Canvas Reference, visit: https://www.w3schools.com/graphics/canvas_reference.asp


# SVG (Scalable Vector Graphics)

## Drawing a Red Square in SVG

In the HTML side only, put:
```HTML5
<svg xmlns="http://www.w3.org/2000/svg" viewbox="0 0 600 600">
  <desc>Red rectangle shape</desc>
  <rect x="10" y="10" width="100" height="100" fill="#c00"  />  
</svg>
```


## Drawing a Yellow Circle with a Green Border in SVG
In the HTML side only, put:
```HTML5
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

## A Sample SVG Logo with a Fiery Gradient
In the HTML side only, put:
```HTML5
<svg height="130" width="500">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="100" cy="70" rx="85" ry="55" fill="url(#grad1)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="50" y="86">SVG</text>
  Sorry, your browser does not support inline SVG.
</svg>
```

For the full SVG Reference, visit: https://www.w3schools.com/graphics/svg_reference.asp



## What's the difference between SVG and Canvas?

* SVG is great for two dimensional graphics.
* SVG uses XML to create vector based 2D graphics - meaning the images are scalable without deteriorating the quality (resolution independent)
* SVG is not suited for gaming.
* You may use programs like Inkscape.com or Adobe Photoshop to generate SVG code for your images
* SVG may be used with JavaScript event handlers.
* SVG graphics use **retained mode** which means you give the object some properties and the browser stores the process to create the image in its memory.
* Canvas uses **immediate mode** which means you, as a developer, need to work out the commands to draw each object to show exactly what you want.  It uses a "Fire and Forget" model, meaning it runs the commands once to display the image and is not aware of the object afterwards.
* Canvas is drawn pixel by pixel.  If the position of an image changes the entire canvas must be changed (see previous bullet).
* Canvas is great for creating 3D graphics
* Canvas is NOT great for high quality resizing of graphics (scalability)
* Canvas requires JavaScript
* Canvas does not render text well
* You can save the resulting image as a PNG or JPG
* Great for graphic intensive games



# Challenge 7

A challenge relating to the original sample code should go here.

```HTML5
// Sample code should that demonstrates what should be taught in this lesson should go here
```

* CRITERIA
    * item
    * item
    * item
