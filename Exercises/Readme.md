# Practical Exercises

#### Use these exercises to challenge and practice what you've learned in your lessons.  These may contain features you'd like to implement into your own portfolio.  It is recommended to attempt these using Codepen.io before implementing into your own designs.



## Table of Contents
### [Big Red Button](#RedButton)
### Vote for Pedro
### ReCreate a Web Page
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

# Vote for Pedro

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
