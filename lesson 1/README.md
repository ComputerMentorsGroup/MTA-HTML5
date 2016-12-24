# Lesson 1

In Lesson one you will learn basic HTML5 tags to create a structure and content for your webpage. 

* Criteria for the Lesson 1 webpage:
    * Must include a title
    * Must use at least two hx (h1-h6) tags
    * Must contain at least one image
    * Must contain at least one paragraph
    * Must include at least one link
    * Must include at least two character entities


```HTML5
<!doctype html>
<html>
    <head>
        <title>78704 Pet Care</title>
    </head>
    <body>
        <h1>Pet Care</h1>
        <img src="assets/dog.jpg">
        <p>Your dog is a friend for life. Why not provide the best care possible?</p>     
        <p>Make sure your pet has plenty of <i><b>fresh water</b></i> during hot weather.</p>
          <p><a href="http://www.google.com">Click here for more information</a></p>
  <br/>
  &copy; Student Name 2017
    </body>
</html>
```
## Details
The code above produces a simple webpage about Pet Care.  The page includes an image, heading tags, paragraphs, and a character entity symbol.  For information about these tags, see the list below.

* `<doctype html>`
    * DOCTYPE declares the document type so the browser can determine what language the document is using.  In this case, we are using HTML, or **HyperText Markup Language**
* `<head><head>`
    * Head tags go at the top of the HTML document.  The head is used for defining the document style and linking to scripts.  Usually the stuff you type in here won't be seen on the page.  Think of it as "behind the scenes".
* `<title></title>`
    * Title tags are the text that shows at the top of your **browser window**, not within the document.  This is also "behind the scenes" and is **nested** within the head tags.  Nested simply means placing a tag within another.
* `<body></body>`
    * Anything you put between the body tags is your actual content, which displays on the webpage document. 
* `<h1></h1>` through `<h6></h6>`
    * Tags h1-h6 provide a variety of header sizes.  h1 is the largest and h6 is the smallest.
* `<b></b>` and `<strong></strong>`
    * Text placed between either sets of these tags is **bolded**  
* `<i></i>` and `<em></em>`
    * Text placed between either sets of these tags is *italicized*
* `<img src="" />`
    * Between the quotes, place the address to an image!  You can do a google search for an image you like, click on it, then copy/paste the web address.  Make sure the web address you're pasting ends with .jpg .jpeg or .png.  This tag is **self-closing** and doesn't have a pair to close it.  Instead, finish the tag simply with a `/>`.
* `<a href="" />` Your clickable text `</a>`
    * Link to other pages or websites using the ANCHOR <a> tag.  HREF stands for
Hypertext REFerence, which is the techy way of saying "Point to this website".  Put
the website address between quotes, and the text you'd like to display (the "Click Me" text) between the <a> tags.
* `<br/>`
    * Another self-closing tag, this is a **line break**.  If you did not need a new paragraph, but simply wanted to insert a new line, use this command.
* `<p></p>`
    * Paragraph tags wrap around blocks of text.  Each paragraph will have a space between the next paragraph.
* `$copy;` and other character entities
    * **Character Entities** are a cool way to use icons on your site.  They begin with the & symbol and end with the ; symbol.  Check out all the different character entities and their code here -https://dev.w3.org/html5/html-author/charref


# Challenge 1

Solve problems found in the code below:

```HTML5
<!doctype html> 
<html>  
  <head>    
    <meta charset="UTF-8">     
    <title>Internal</title>  
  </head>
<body> 
  <h1>Staff Meeting</h1> 
  <img src="assets/cologo" olt="Company logo" /> 
  <p>Report to the <strong>Blue Conference Room</strong> at <strong>10:00 a.m.</strong> on <strong>Thursday</strong>
    <strong>for an emergency staff meeting.</strong></p> 
  
  <h3>Meeting Agenda<h3>
   
  <p><strong>For the meeting agenda, please click the link below:</strong></p>
  <p><a "http://computermentors.org/">Agenda Link </a> </p>

</body> 
</html>
```

* CRITERIA:
    * When hovering over the image the text "Company Logo" should pop up.
    * The words "for an emergency staff meeting" should no longer be bold.
    * The logo should appear.
    * The text "For the meeting agenda, please click the link below:" should be italic, not bold.
    * The text "Agenda Link" should be linked properly
    * "Meeting Agenda" should be same size as "Staff Meeting"


