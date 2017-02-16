# Lesson 6

In Lesson Num you will learn Advanced CSS topics, especially as they relate to transforming and drawing objects on the screen.

### Instructions
1. Open Notepad, or your favorite text editor.
2. Save the file as greetings.html
3. Open a second Notepad Window
4. Save the second window as style.css
5. Using the example below, reproduce the webpage with your own content to create a greeting card for any occasion of your choice.

**Need an idea?  Pick from these greetings:**
* Birthday Card
* Thinking of You
* Christmas Card
* Be My Valentine
* Thank You

**Criteria for the Lesson 6 webpage:**
* Create a greeting that uses any transform effect.
* Create a message that uses keyframe animations.
* Include one additional element you've learned previously (such as video, audio, lists, tables, buttons, links, etc)
* Have two separate files, one for HTML and another for CSS

Use the following code for greeting.html file:
```HTML5
<!DOCTYPE html>
<html>

<head>
   <title>Merry Christmas Greeting Card</title>
   <link href="https://fonts.googleapis.com/css?family=Great+Vibes" rel="stylesheet">
   <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
   <div class="container">
	   <div class="greeting">Merry Christmas</div>
	   <div class="message">With Love, <br/> The Frisco Family</div>

	
      <audio autoplay controls id="winterSong"> 
         <source src="http://mfrisco.github.io/winter16/assets/we-wish-you-a-merry-christmas.mp3">
         <source src="http://mfrisco.github.io/winter16/assets/we-wish-you-a-merry-christmas.ogg">
	      Your browser does not support audio for this webpage!
		</audio>
   </div>
</body>
</html>
```

## Details
Details about what the code above goes here

* `Each line of code should be bulleted here`
    * A bulleted list of things about the line above should go here
    * **Really important stuff should be bold like this**
    * Keywords should be *italicized*


# Challenge 6

 What would you change in the CSS file to animate the red box to move up? 

```HTML5
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width">
<title>repl.it</title>
</head>
<html>
<style>
   #boxStyle {
   -ms-animation-name: moveUp;
   -ms-animation-duration: 5s;
   -webkit-animation-name: moveUp;
   -webkit-animation-duration: 5s;
   animation-name: moveUp;
   animation-duration: 5s;
   width: 200px;
   height: 20px;
   position: relative;
   left: 0px;
   top: 0px;
   background-color: red;
   text-align: center;
   color: white;
   font-family: arial;
   padding: 1em;
   }

   @-ms-keyframes moveUp {
   0% { }
   100% { top: 0px; }
   }
   
   @-webkit-keyframes moveUp {
   0% { }
   100% { top: 0px; }
   }
   
  @-keyframes moveUp {
   0% { }
   100% { top: 0px; }
   }
</style>

<body>
<div id="boxStyle">Hello!</div>
</body>
</html>
```

Complete Challenge 6 on Repl.it: https://repl.it/classroom/invite/CJuYkDU
