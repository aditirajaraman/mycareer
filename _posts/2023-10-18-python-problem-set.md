---
title: "Meeting #2 Problem Set!"
date: 2024-01-02T15:34:30-04:00
categories:
  - code
tags:
  - python
  - programming
---

1. Create a function that checks if a given number is a prime number. The function should return True if the number is prime and False otherwise.

```
def prime(num):
    if num < 2:
        print("False")
    for i in range(2,int(num**0.5) + 1):
        if num % i == 0:
            print("False")
        else:
            print("True")

print(prime(13))
```

2. Create a Calculator with methods to perform basic arithmetic operations: add, subtract, multiply, and divide. Each method should take two numbers as parameters and return the result of the operation.

```
def add(num1, num2):
  print(num1 + num2)

def sub(num1, num2):
  print(num1-num2)

def mult(num1, num2):
  print(num1*num2)

def div(num1, num2):
  print(num1/num2)
```

3. Create two methods which take the weather in Fahrenheit and return it to Celsius and vice versa. Each method takes one number as a parameter  and returns the result. 
```
def C_to_F(C):
  print(C* (9/5+32))

def F_to_C(F):
  print((F-32)*5/9)

print(F_to_C(56))
```