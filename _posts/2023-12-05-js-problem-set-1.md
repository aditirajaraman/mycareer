---
title: "Javascript Problem Set 1"
date: 2023-12-12T15:34:30-04:00
categories:
  - code
tags:
  - programming
  - javascript
---

// 1. Define a variable called math that stores the integer 2 and prints out this variable.<br>
<i>
var math = 2;<br>
console.log(math);<br>
</i>

// 2. Define a variable word such that it stores the string "Hello!" and print out this variable on the document.<br>
<i>
var word = "Hello!";<br>
document.write(word);<br>
</i>

// 3. Define a variable isFalse such that it stores the value False and print out this variable as an alert.<br><i>
var isFalse = false;<br>
alert(isFalse);<br>
</i>

// 4. Define a variable decimal such that it stores the float 2.00001 and print out this variable in the console.<br><i>
var decimal = 2.00001;<br>
console.log(decimal);<br></i>

// 5. Print this statement as an alert using casting with integer, string, and boolean variables: “ True: I ate 6 cookies.”<br><i>
var cookies = 6;<br>
alert("True: I ate " + cookies + " cookies.");<br></i>

// 6. Create a program that asks the user to enter their name and their age. Then print out a message saying "Your name is (input name) and you are (input age) years old"<br><i>
var userName = prompt("Enter your name:");<br>
var userAge = prompt("Enter your age:");<br>
console.log("Your name is " + userName + " and you are " + userAge + " years old.");<br></i>

// 7. Create a program that asks the user to enter their name and their age. Print out a message as an alert addressed to them that tells them the year that they will turn 100 years old.<br><i>
var userAgeInput = prompt("Enter your age:");<br>
var currentYear = new Date().getFullYear();<br>
var yearToTurn100 = currentYear + (100 - parseInt(userAgeInput));<br>
alert("Hello, " + userName + "! You will turn 100 in the year " + yearToTurn100 + ".");<br></i>





[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
