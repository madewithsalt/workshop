---
layout: post
title: "Calculator"
date: 2014-10-04 16:21:42 -0400
comments: true
summary: "Practice functions in JavaScript with a simple calculator."
categories: ["Beginner JS"]
---

## The Calculator
You can use something like [repl.it](http://repl.it) to code this so that you don't need to worry about making a webpage, or you can create a whole webpage for it, with inputs and buttons. You may want to start off with just JS and then add the UI later, but it's up to you.

You may find [these slides](http://www.teaching-materials.org/javascript/slides/varsfunctions.html) useful.

- Write a function called `squareNumber` that will take one argument (a number), square that number, and return the result. It should also log a string like `"The result of squaring the number 3 is 9."`
- Write a function called `halfNumber` that will take one argument (a number), divide it by 2, and return the result. It should also log a string like `"Half of 5 is 2.5."`
- Write a function called `percentOf` that will take two numbers, figure out what percent the first number represents of the second number, and return the result. It should also log a string like "2 is 50% of 4."
- Write a function called `areaOfCircle` that will take one argument (the radius), calculate the area based on that, and return the result. It should also log a string like `"The area for a circle with radius 2 is 12.566370614359172"`
- **Bonus:** Round the result so there are only two digits after the decimal.
- Write a function that will take one argument (a number) and perform the following operations, using the functions you wrote earlier:
  - Take half of the number and store the result.
  - Square the result of #1 and store that result.
  - Calculate the area of a circle with the result of #2 as the radius.
  - Calculate what percentage that area is of the squared result (#3).


### [See Solution](/files/beg_js/calculator_solution.js)
