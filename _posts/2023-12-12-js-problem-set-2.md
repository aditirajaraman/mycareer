---
title: "Javascript Problem Set 2"
date: 2023-12-12T15:34:30-04:00
categories:
  - code
tags:
  - programming
  - javascript
---

//1. Using the user's input for n, make a for loop to print all the odd numbers up to and including n (not including 0).<br>
var n = prompt("Enter a number: ");<br>
for(var i = 1; i <= n; i++){<br>
  if(i%2!==0){<br>
    console.log(i);<br>
  }<br>
}<br>
//2. Using the user's input for y, calculate and print the factorial of the number.<br>
//Ex: if y = 4, return the answer to 4*3*2*1 <br>
var y = prompt("Enter a number: ");<br>
for(var i = y-1; i > 1; i--){<br>
  y *= i;<br>
}<br>
console.log(y);<br>

//3. Using user input for a number (num), find the sum of every number from 1 to num. The number will always be a positive integer greater than 0.<br>
//Ex: <br>
var num = prompt("Enter a number: ");<br>
var sum = 0;<br>
for(var i = 1; i <= num; i++){<br>
  sum+=i;<br>
}<br>
console.log(sum);<br>

//4. Write a program that will allow someone to guess a five digit pin exactly 5 times. If the user guesses the number correctly. It prints “That was correct!” Otherwise it will print “Sorry that was wrong.” Program stops after the 5th attempt or if they got it right.<br>
var pin = 39248;<br>
for(var i = 0; i<5; i++){<br>
  var attempts = prompt("Guess a 5 digit pin: ");<br>
  if (attempts == pin){<br>
    console.log("That was correct!");<br>
    break;<br>
  }<br>
  else{<br>
    console.log("Sorry that was wrong.");<br>
  }<br>
}<br>

//5. Make a program which uses a for loop with a range of 90. Your loop should go through the numbers 0-90 and print butter if the number is divisible by 4, fly if the number is divisible by 7, and butterfly if the number is divisible by both 3 & 5.<br>
for(var i = 0; i <= 90; i++){<br>
  if(i % 4 == 0 && i % 7 == 0){<br>
    console.log(i + " butterfly");<br>
  }<br>
  else if(i % 7 == 0){<br>
    console.log(i + " butter");<br>
  }<br>
  else if (i % 4 == 0){<br>
    console.log(i + " fly");<br>
  }<br>
}<br>

//6. Make a program which takes in an integer and uses a while loop to print the times table of that integer up til the number 12 in the console.<br>
//Ex. If user enters 4, program prints 4....48<br>
var num = prompt("Enter a number: ");<br>
var i = 1;<br>
while (i <= 12){<br>
  console.log(i*num);<br>
  i++;<br>
} <br>

//7. Create a function which takes in a base and an power and returns the exponent without using the ** operation. <br>
// hint: use a for loop<br>

function power(a,b){<br>
  var num=0;<br>
  for(var i=1;i<b;i++){<br>
    num += a*a;<br>
  }<br>
  return num;<br>
}<br>
console.log(power(2,3));<br>

//8. Create a function which takes in an integer and returns the absolute value.<br>
<br>
function absolute(a){<br>
  if (a>0) {<br>
    return a;<br>
  }<br>
  else {<br>
    return -a;<br>
  }<br>
}<br>
console.log(absolute(-4));<br>

//9.  A quadratic equation ax² + bx + c = 0 has either 0, 1, or 2 distinct solutions for real values of x. Given a, b and c, you should return the number of solutions to the equation.<br>
// hint: use the equation b²-4ac; if result is <0, then 0 real solutions, if result is =0, then 1 solution, & if result>0, then 2 solutions<br>

function solutions(a,b,c){<br>
  var x = b**2 - 4*a*c;<br>
  if (x > 0){<br>
    return "2 real solutions";<br>
  }<br>
  else if(x==0){<br>
    return "1 real solution";<br>
  }<br>
  else{<br>
    return "no real solutions";<br>
  }<br>
}<br>
console.log(solutions(6, -17, 12));<br>

//10.  Create a function which takes in a number n and returns the nth factorial <br>
// ex. if n=5, return 5*4*3*2*1<br>

function factorial(n){<br>
  for (var i=n-1;n>=1;n--){<br>
    n*=i;<br>
  }<br>
  return n<br>
}<br>
console.log(factorial(4));<br>





[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
