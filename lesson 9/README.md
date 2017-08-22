# Lesson 9

In Lesson 9, you will explore form-database interactions. Sending and receiving data in these interactions relies on SQL. SQL stands for Structured Query Language and is used to communicate with databases. We will be using the Cloud 9 platform to setup a database to interact with your form.
 
### Instructions
1. Visit https://c9.io and create an account
2. Before filling out any "Billing" info, the Mentor will login and add your account to the TeenTech Workspace https://c9.io/team/stemcorps/manage
3. Follow the instructions provided carefully. If any problems arise, contact your instructor.


### PART I:
**Create and style a form using HTML and CSS.  This form will be used to collect information.  You may use any fields you wish!

**Criteria for the Lesson 9 webpage:**
* Create a form
* Apply styling to buttons and fields
* The form must look visually appealing.

HTML:
```HTML5
<form name="Roster" action="db.php" method="post" onsubmit="required()" />
<p><input type="text" name="StudentName" placeholder="Your Full Name" /></p>
<p>
<select name="Location">
  <option value="">Select a Location</option>
  <option value="HIVE">HIVE Downtown Tampa</option>
  <option value="CMG MLK">CMG on MLK</option>
  <option value="Brandon Rec">Brandon Community Center</option>
  <option value="SouthShore Library">SouthShore Library</option>
  <option value="Seminole Heights Library">Seminole Heights Library</option>
  <option value="Middleton HS FBLA">Middleton H.S. FBLA</option>
  <option value="WUCHS">West University Charter H.S.</option>
</select>
</p>
<input type="submit" value="Submit" />
</form>

```

CSS (Style):
(How could you improve the CSS to make the form look better?)
```CSS
* {
    text-align: center;
}

input[type=text] {
    font-family: Georgia;
}

input[type=submit] {
    border-radius: 10px;
}

select {
    font-size: 1em;
    
}
```


### PART II:


## Details
Details about what the code above goes here

* `Each line of code should be bulleted here`
    * A bulleted list of things about the line above should go here
    * **Really important stuff should be bold like this**
    * Keywords should be *italicized*


# Challenge Num

A challenge relating to the original sample code should go here.

```HTML5
// Sample code should that demonstrates what should be taught in this lesson should go here
```

* CRITERIA
    * item
    * item
    * item
