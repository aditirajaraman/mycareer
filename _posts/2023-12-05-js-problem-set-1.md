---
title: "Javascript Problem Set 2"
date: 2023-12-12T15:34:30-04:00
categories:
  - code
tags:
  - programming
  - javascript
---

 1. Using the user's input for n, make a for loop to print all the odd numbers up to and including n (not including 0).

```
var n = parseInt(prompt(“Enter a number:”));

for (var i = 1; i <= n; i++) {
  if (i % 2 != 0) {
    console.log(i);
  }
}

```

 2. Using the user's input for y, calculate and print the factorial of the number. ex. if y = 4, return the answer to 4*3*2*1 

```
var y = parseInt(prompt(“Enter a number:”));

var f = 1;
for (var i = 1; i <= y; i++) {
  f = f * i;
}

console.log(f);

```

 3. Write a program that finds the summation of every number from 1 to num. The number will always be a positive integer greater than 0.
```
var num = parseInt(prompt("Enter a number:"));
var sum = 0;
for (var i = 1; i <= num; i++) {
  sum = sum + i;
}
console.log(sum);

```

 4. Write a program that will allow someone to guess a four digit pin exactly 4 times. If the user guesses the number correctly. It prints “That was correct!” Otherwise it will print “Sorry that was wrong.” Program stops after the 4th attempt if they got it righ
```
var pin = "3459"; 
var tries = 0;

while (tries < 4) {
  var guess = prompt("Guess the 4-digit pin:");
  if (guess == pin) {
    console.log("That was correct!");
    break;
  } else {
    console.log("Sorry that was wrong.");
    tries++;
  }
  
}

```


 5. Make a program which uses a for loop with a range of 90. Your loop should go through the numbers 0-90 and print butter if the number is divisible by 4, fly if the number is divisible by 7, and butterfly if the number is divisible by both 3 & 5.
```
for (var i = 0; i <= 90; i++) {
  if (i % 3 == 0 && i % 5 == 0) {
    console.log("butterfly");
  } else if (i % 4 == 0) {
    console.log("butter");
  } else if (i % 7 == 0) {
    console.log("fly");
  } else {
    console.log(i);
  }
}

```


 6. Make a program which takes in an integer and uses a while loop to print the times table of that integer up til the number 15 in the console. Ex. If user enters 4, program prints 4....60

```
var num = parseInt(prompt("Number: "));
var i = 1;
while (i < 16){
console.log(num*i)
i++;
}

```


 7. Create a function which takes in a base and a power and returns the exponent without using the ** operation. hint: use a for loop

```
function power(base, exp) {
  var result = 1;
  for (var i = 0; i < exp; i++) {
    result = result * base;
  }
  return result;
}
console.log(power(2, 3));

```


8. Create a function which takes in an integer and returns its absolute value.

```
function absolute_value(x) {
  if (x < 0) {
    return -1 * x;
  } else {
    return x;
  }
}

```


9.  A quadratic equation ax² + bx + c = 0 has either 0, 1, or 2 distinct solutions for real values of x. Given a, b and c, you should return the number of solutions to the equation. hint: use the equation b²-4ac; if result is <0, then 0 real solutions, if result is =0, then 1 solution, & if result>0, then 2 solutions

```
function sol(a, b, c) {
  var disc = Math.pow(b, 2) - (4 * a * c);
  if (disc < 0) {
    return 0;
  } else if (disc == 0) {
    return 1;
  } else {
    return 2;
  }
}

```






[jekyll-docs]: https:jekyllrb.com/docs/home
[jekyll-gh]:   https:github.com/jekyll/jekyll
[jekyll-talk]: https:talk.jekyllrb.com/
