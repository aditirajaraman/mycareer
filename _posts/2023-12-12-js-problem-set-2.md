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
var n = prompt("Enter a number: ");
for(var i = 1; i <= n; i++){
  if(i%2!==0){
    console.log(i);
  }
}
```
2. Using the user's input for y, calculate and print the factorial of the number.
> Ex: if y = 4, return the answer to 4*3*2*1 
```
var y = prompt("Enter a number: ");
for(var i = y-1; i > 1; i--){
  y *= i;
}
console.log(y);
```

3. Using user input for a number (num), find the sum of every number from 1 to num. The number will always be a positive integer greater than 0.
> Ex:
var num = prompt("Enter a number: ");
var sum = 0;
```
for(var i = 1; i <= num; i++){
  sum+=i;
}
console.log(sum);
```

4. Write a program that will allow someone to guess a five digit pin exactly 5 times. If the user guesses the number correctly. It prints “That was correct!” Otherwise it will print “Sorry that was wrong.” Program stops after the 5th attempt or if they got it right.
```
var pin = 39248;
for(var i = 0; i<5; i++){
  var attempts = prompt("Guess a 5 digit pin: ");
  if (attempts == pin){
    console.log("That was correct!");
    break;
  }
  else{
    console.log("Sorry that was wrong.");
  }
}
```

5. Make a program which uses a for loop with a range of 90. Your loop should go through the numbers 0-90 and print butter if the number is divisible by 4, fly if the number is divisible by 7, and butterfly if the number is divisible by both 3 & 5.
```
for(var i = 0; i <= 90; i++){
  if(i % 4 == 0 && i % 7 == 0){
    console.log(i + " butterfly");
  }
  else if(i % 7 == 0){
    console.log(i + " butter");
  }
  else if (i % 4 == 0){
    console.log(i + " fly");
  }
}
```

6. Make a program which takes in an integer and uses a while loop to print the times table of that integer up til the number 12 in the console.
> Ex. If user enters 4, program prints 4....48
```
var num = prompt("Enter a number: ");
var i = 1;<
while (i <= 12){
  console.log(i*num);
  i++;
} 
```

7. Create a function which takes in a base and an power and returns the exponent without using the ** operation. 
> hint: use a for loop
```
function power(a,b){
  var num=0;
  for(var i=1;i<b;i++){
    num += a*a;
  }
  return num;
}
console.log(power(2,3));
```

8. Create a function which takes in an integer and returns the absolute value.
```
function absolute(a){
  if (a>0) {
    return a;
  }
  else {
    return -a;
  }
}
console.log(absolute(-4));
```

9.  A quadratic equation ax² + bx + c = 0 has either 0, 1, or 2 distinct solutions for real values of x. Given a, b and c, you should return the number of solutions to the equation.
> hint: use the equation b²-4ac; if result is <0, then 0 real solutions, if result is =0, then 1 solution, & if result>0, then 2 solutions
```
function solutions(a,b,c){
  var x = b**2 - 4*a*c;
  if (x > 0){
    return "2 real solutions";
  }
  else if(x==0){
    return "1 real solution";
  }
  else{
    return "no real solutions";
  }
}
console.log(solutions(6, -17, 12));
```

10.  Create a function which takes in a number n and returns the nth factorial 
> ex. if n=5, return 5*4*3*2*1
```
function factorial(n){
  for (var i=n-1;n>=1;n--){
    n*=i;
  }
  return n
}
console.log(factorial(4));
```