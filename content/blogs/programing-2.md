---
title: "Minimum, chapter 3 Eloquent JavaScript"
description: ""
omit_header_text: true
summary: "Programming article 2."
type: page
tags: [JavaScript, problem]
category: [substantive]
---
## Introduction to the Problem
I'm showing a problem and a solution shown in Chapter 3 of *Eloquent JavaScript* by *Marijn Haverbeke*.  See Eloquent JavaScript, Chapter 3 [here](https://eloquentjavascript.net/03_functions.html)

Below is the question.
<blockquote>
The previous chapter introduced the standard function Math.min that returns its smallest argument. We can write a function like that 
ourselves now. Define the function min that takes two arguments and returns their minimum.
</blockquote>

## My solution:
```js
function min(x,y){
    if (x > y){
        return y
    } else {
        return x
    }
}
console.log(min(0, 10))
console.log(min(0, -10))
```
<button id="runMin">Run Min</button>

<pre id="outputMin" style="background:#f4f4f4; color:black; padding:1rem; border-radius:5px; max-height:300px; overflow:auto;"></pre>

<script>
document.getElementById("runMin").addEventListener("click", () => {
  const output = document.getElementById("outputMin");
  output.textContent = ""; 
  function min(x,y){
    if (x > y){
        return y;
    } else {
        return x;
    }
  }
  output.textContent += min(0, 10) + "\n";
  output.textContent += min(0, -10) + "\n";
});
</script>


## Creating a function
* A **function** is created with an expression that starts with the keyword *function (Eloquent JavaScript chapter 3)*.
* In this example, the function is named *min*.
* A function can take zero, one, or multiple **parameters** and has a **body**, that contains the statement to be executed when the function is called *(Eloquent JavaScript chapter 3)*. 
* Here, the parameters are x and y, representing the two values we want to compare.

## The body of the function
* If statement:
    - The function uses an if statement, which allows a piece of code to run only when a specific condition is true. *(Eloquent JavaScript, Chapter 3)*
* The first if statement created has the **Boolean expression**: 
```js
x > y
```
* The **>** operator means *greater than*, so the expression is only true if x is bigger then y.
* If the expression is true the function will execute the following statement. In this case it is **return y**. This will return y because it is the smaller of the two values.
* The function is followed by an **else** and the statement to execute **return x**. This means that if the previous Boolean expression is false and x will be the number that is returned because it is the smallest.

## Calling the function
* We call the function by using:
``js
console.log(min(0, 10))
``
* **console.log ()** is a function that writes out its arguments to some text output device (eloquent JavaScript chapter 2).
* To call the function, we write its name followed by parentheses containing the values we want to pass as arguments.
* In this case, we are comparing the number 0 and 10 in the function min. It returns the smaller value, and console.log() then prints that result.