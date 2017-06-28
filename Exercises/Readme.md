# Practical Exercises

#### Use these exercises to challenge and practice what you've learned in your lessons.  These may contain features you'd like to implement into your own portfolio.  It is recommended to attempt these using Codepen.io before implementing into your own designs.



## Table of Contents
### [Big Red Button](#RedButton)
### [Vote for Pedro](#Pedro)
### [My Resume](#resume)
### Forms
### Sending and Retrieving Data
### Fun with Canvas
### Fun with SVG

***

# Big Red Button <a name="RedButton"></a>

## HTML
```HTML5
<button onclick="message()">Don't</button>
```

## CSS
```HTML5
button {
  height: 200px;
  width: 200px;
  border-radius: 200px;
  background: red;
  color: white;
  font-family: Impact;
  font-size: 40pt;
  text-transform: uppercase;
  }

```

## JS
```JavaScript
function message() {
  alert('Oh No!');
  }
```
***

# Vote for Pedro <a name="Pedro"></a>

## HTML
```HTML5
<button onclick="clickMe()">Vote</button>
<p>Votes: <a id="clicks">0</div></p>
```

## CSS
```HTML5
button {
  height: 200px;
  width: 200px;
  border-radius: 200px;
  background: red;
  color: white;
  font-family: Impact;
  font-size: 40pt;
  text-transform: uppercase;
  }

button:hover {
  background: blue;
  transition: .5s;
}
```


## JS
```HTML5
  var clicks=0;
  function clickMe(){
    clicks += 1;
    document.getElementById("clicks").innerHTML = clicks;
  }
```

***

# My Resume <a name="resume"></a>

## HTML
```HTML5
<h1>My Name</h1>
<h3><a href="mailto:myemail@domain.com">MyEmail@domain.com</a></h3>

<h2>About</h2>
<p>Describe who you are and what you are looking for in a workplace.</p>

<h2>Education</h2>
<h3>West University High School</h3>
<h3>Graduated May 2017</h3>


<h2>Skills and Abilities</h2>
<ul>
<li>Certification in Microsoft Office PowerPoint 2013</li>
<li>Certified Microsoft Technology Associate, Software Development in C#</li>
<li>Customer Service Oriented</li>
</ul>
```

## CSS
```HTML5
/* Importing Google.com Font called Exo */
@import url('https://fonts.googleapis.com/css?family=Exo');

body {font-family: Arial;
margin: 0 200px;}

.intro {
	text-align: center;}

img {
	display: inline-block; 
	margin: auto;
	vertical-align: middle;
	height: 200px;
	width: 300px;
	border-radius: 160px;
}

h1 {text-align: center;
font-family: 'Exo', sans-serif;}

h2 {margin-top: 50px; /* Adding a little space between previous section's content and heading*/
	font-family: 'Exo', sans-serif;
	color: #ffffff;
	background: #1693A5;
	padding: 8px;
	width: 250px;}

h3 {text-align: center;
	line-height: .8em;
}

/* Changing link color and remove underline */
a:link, a:visited, a:active {
color: #1693A5;
text-decoration: none;}

/* Link Hover color and H2 Hover - timed transition to fade color in*/
a:hover, h2:hover {color: #000000; 
	transition: .7s;}

```

