---
title: "FizzBuzz, chapter 2 Eloquent Javascripte"
description: ""
omit_header_text: true
summary: "Programming article 1."
type: page
weight: 2
tags: [javascrips, problem]
---
## Introduction to the Problem
We describe a solution, written in JavaScript and executed in the Node.js environment, to the *FizzBuzz* problem.  

The problem is showen in Chapter 2 of *Eloquent JavaScript* by *Marijn Haverbeke*.  

In summary, the program prints the numbers from 1 to 100, with three exceptions:

- For numbers divisible by 3, print `"Fizz"` instead of the number.  
- For numbers divisible by 5 (but not 3), print `"Buzz"`.  
- For numbers divisible by both 3 and 5 prints `"FizzBuzz"`.  

# my solution:
```
let num = 1; 
while(num <= 100) {
  if (num % 3 === 0 && num % 5 === 0){
    console.log("FizzBuzz");
  } else if (num % 3 === 0 ) { 
    console.log("Fizz"); 
  } else if (num % 5 === 0 ) { 
    console.log("Buzz"); 
  } else{
    console.log(num);
  }
  num++;
}
```
# concepts
-	Console.log (): function that writes out its arguments to some text output device (eloquent JavaScript)
-	Loop: 
>	a form of flow control that runs a piece of code multiple times 
*	Looping control flow allows us to go back to some point in the program where we were before and repeat it with our current program state. 
-	If statement:
*	The code will only be executed if, and only if, a certain condition id true device (eloquent JavaScript)
*	The if keyword executes or skips a statement depending on the value of the Boolean expression (eloquent JavaScript)
If (expression) {
Statement to execute}
-	While: 

While (expression) {
If statement {} else if statement {}}
-	%:

-	Value_name ++:
*	Value_name = value_name + 1;
*	Means that we are adding one more to the value present
-	Let:
*	binding 
*	Binding defines a value to a name that can be used in an expression




