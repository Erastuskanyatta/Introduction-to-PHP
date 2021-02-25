### GETTING STARTED WITH PHP
[PHP](stuff-here) (Hypertext Pre-processor) is a web server-side programming language. It allows developers to create web applications that interact with a database.

### Why PHP?
PHP can be used to do many things. Let us look at some examples of how PHP is used:
1. PHP is platform-independent. This means that it runs on all operating systems. ie. Mac OS, Windows, or Linux.
2. It can run on all modern servers eg. Apache
3. PHP can be integrated with databases like [MariaDb]({}).
4. Easy to learn and put in place.
5. PHP frameworks are used to build web applications. Here are some of the most popular PHP frameworks.
 1. [Yii 2]({}) {}
 2. [Laravel](https://laravel.com/) {}
 3. [FuelPHP](https://fuelphp.com/) {}
 
### Prerequisites
Before you start this article, make sure you have  [Xampp](https://www.apachefriends.org). You can download Xampp [here](https://www.apachefriends.org/download.html). **In this article, we will use Ubuntu**. A folder ```/opt/lampp``` will be created after your done with the installation.
{starting Xampp}

### Creating PHP files
Navigate to ```/opt/lampp/htdocs``` and create a new folder ```hello``` where we will have our PHP files. Open a terminal and run the command below.

```bash
$ cd /opt/lampp/htdocs
$ sudo mkdir hello
$ cd hello
```
Then, create a new file ```index.php``` in ```/opt/lampp/htdocs/hello```. Run the following command in the terminal.
```bash
$ sudo touch index.php
```
Then, open the file using [Gedit](https://wiki.gnome.org/Apps/Gedit) by running the following command.
```bash
$ sudo gedit index.php
```
### A hello world program
We are going to write a simple PHP program.Let's look at the basic syntax of a PHP program. PHP code starts with `<?php` and ends with `?>` as shown below:
```php
<?php
//php code is written here
?>
```
In the ```index.php``` file you created above put the following code:
```php
<?php
 echo "<h1>Hello world!</h1>";
?>
```
We use the `echo` statement is to display output on the screen. We use this statement to display an Html heading.

To run this code, open your browser at http://localhost/hello. Here, we append the folder name .ie `hello` to the base URL http://localhost/.

You should see something like this image on your browser:
![php](helloworld.png)

Congratulations! You have written your first PHP program.
### Variables in PHP

### Conditional statements in PHP
Condition Statements can be used to perform different types of actions. They include :

- `if` statement - used to execute some code if a given condition is true.
- `if... else` statement -  the `if` block is used to execute some code if a certain condition is true. If the condition is false, then the `else` block executes another block of code.
This statement executes either true or false code depending on the condition. This means that this statement contains two conditions.

- `if... else if...else` statement - It is like the `if ...else` statement, but with the ability to check for many conditions.

Let us implement each of the statement above:

### 1. the `if` statement
The syntax of an `if` statement looks like this.
```php
if(condition){
 //code to execute
}
```
Let us implement this in a program.
```php
<?php
$age = 15;

if ($age < 18) {
 echo "a kid!";
}
?>
```
Running this code gives `a kid!` as the output.

<!-- From the above example we have:
- $age = 15; - variable $age is defined and a value 15 is assigned to it.
In PHP, Variables are declared by first writing the $sigh followed by the name of the variable.
- if (`$age < "18"`)- this the condition to be followed.
- echo "you are a kid!"- this will be the output if the condition is true -->

### 2. ````if...else```` statement 

syntax
```php
if(condition){
 //code to execute if condition is true
}
else{
 //code to execute if condition is false
}
```
A simple implementation of the above would look like this:
```php
<?php
$age = 18;
if($age < 18){
 echo "a kid!";
}
else{
 echo "so youth!";
}
?>
```
The output should be: ``so youth!``. This is because the ``age`` is not less than 18. If we assign a value like 17 to variable ``age`` the output should be ```a kid!```

### 3. `if...elseif...else` statement
The syntax of this statement looks as shown below.
```php
if (condition) {
 // code to execute if condition is true;
} elseif (condition_2) {
 // code to execute if condition_2 is true
} else {
 // code to execute if none of the above are true
}
```
Implementing the above would look like like this:
```php
<?php
$age = "18";

if($age < "18"){
 echo "a kid!";
}
elseif($age > "35"){
 echo "a parent?";
}
else{}
 echo"a youth!";
?>
```
Since the ``` age``` is equal to ``18`` the output of the following code should be: ```a youth!```.
### Comments In PHP
Commenting in PHP may be done for many reasons. For example, it can a person reading the code to understand it. A commented line is not executed as a part of the program. There are 2 types of comments.

### 1. Single line comment

This is a comment spanning a single line. Look at the example below.
```php
<?php
 // this is an example of a single-line comment.
 echo"The output is:";
 # this is another one.
?>
```
As shown above, you can use 2 backslashes (````//````) or a hashtag (```#```) for single-line comments. 

### 2. Multiple-line comment
This is a comment spanning multiple lines. Here, you can use the symbols `/*` to open and `*/` to close the comment as shown below.
```php
<?php
 echo "hello!!"
 /*
  This is a comment,
  that should span multiple lines
  */
?>
```
### Conclusion
In this tutorial, we have looked at the following:
- Basic PHP program syntax
- Variables in PHP
- Conditional statements
- Comments in PHP

## Have good PHP coding ahead