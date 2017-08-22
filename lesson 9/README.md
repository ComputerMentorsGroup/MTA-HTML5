# Lesson 9

In Lesson 9, you will explore form-database interactions. Sending and receiving data in these interactions relies on SQL. SQL stands for Structured Query Language and is used to communicate with databases. We will be using the Cloud 9 platform to setup a database to interact with your form.
 
### Instructions
1. Visit https://c9.io and create an account
2. Before filling out any "Billing" info, the Mentor will login and add your account to the TeenTech Workspace https://c9.io/team/stemcorps/manage
3. Follow the instructions provided carefully. If any problems arise, contact your instructor.


## PART I:
**Create and style a form using HTML and CSS.  This form will be used to collect information.  You may use any fields you wish!**

**Criteria for the Lesson 9 webpage:**
* Create a form in an **index.html** file
* Apply styling to buttons and fields
* The form must look visually appealing.

HTML:
```HTML
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


## PART II:

**Establish a MySQL Database**
1. Click the **bash** tab at the bottom of the c9.io interface
2. We will use the commands as described here: https://docs.c9.io/docs/setup-a-database and below:
3. Type: **mysql-ctl install** and press **enter**
4. Write down the username and password in a safe place
5. Type: **show databases;** and press **enter**
6. Since we will be using the c9 database, type **use c9;** and press **enter**
7. Type: **show tables;** and press **enter**

#### We do not have any tables yet!  A table is what holds and organizes the structure of data after it has been submitted via the form.  There are lots of tables within a database which share and link information together.  For example, one table may hold a list of products, another table may hold a list of customers, and a third table may hold all of the orders, linking products and customers together.

The command to create a table looks like this, in concept:
CREATE TABLE table_name (
    column1 datatype constraint,
    column2 datatype constraint,
    column3 datatype constraint,
    ....
);

The **datatype** could mean it's a string of text (varchar), a number that (int), timestamp, or many other things!  For more info on datatypes, visit: http://www.cs.toronto.edu/~nn/csc309/guide/pointbase/docs/html/htmlfiles/dev_datatypesandconversionsFIN.html


8. Let's continue using the example form we created previously.  Type the following, using *SHIFT+ENTER* to go down each line.  Press **ENTER** at the very end.

CREATE TABLE Demo (

  id int(6) PRIMARY KEY AUTO_INCREMENT UNIQUE,
  
  StudentName VARCHAR(120),
  
  Location VARCHAR(120),
  
  ClassDate TIMESTAMP);

#### In our example scenario, each student who signs in via the form would be given an ID and a TIMESTAMP, issued when the submit button is pressed and the entry is stored into the table we just made.  


9.  Now create a table that uses all of your form inputs!  Must include the following:
* ID using a Primary Key
* Timestamp
* All fields within your form

#### We've created a form and established a database, but we still need to connect the form to the database!  See Part III.




## PART III:

1. In Cloud 9 (c9.io), create a file (File-New File) named: **db.php**
2. Here we will use a language called PHP to make the Form->Database connection.  There are other languages that may do this, such as Node.JS, but for this section we will demonstrate PHP.



```PHP
<?php

define('DB_NAME', 'c9');
define('DB_USER', 'username');
define('DB_PASSWORD', '');
define('DB_HOST','localhost');

$link = mysql_connect(DB_HOST, DB_USER, DB_PASSWORD);

if (!$link) {
    die('Could not connect: ' . mysql_error());
}

$db_selected = mysql_select_db(DB_NAME, $link);
 
if (!$db_selected) {
    die('Can\'t use ' . DB_NAME . ': ' . mysql_error());
}


$value = $_POST['StudentName'];
$value2 = $_POST['Location'];

/*Insert into DB */
$sql = "INSERT INTO Demo (StudentName, Location) VALUES ('$value', '$value2')";


if (!mysql_query($sql)) {
    die('Error: ' . mysql_error());
}


mysql_close();
?>

<style>
body {font-family: verdana;}
</style>
<body>
<h1>Submission Received!</h1>
<p><a href="index.html">(Go Back)</a></p>
</body>
```

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
