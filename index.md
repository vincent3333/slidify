---
title       : Fibonacci Sequence
subtitle    : Auto-caculating the fibonacci sequence you enter.
author      : Vincent Chang
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax,bootstrap, shiny, interactive]     
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## What is the "Fibonacci Sequence" 

In mathematics, the Fibonacci numbers or Fibonacci sequence are the numbers in the following integer sequence:

1,1,2,3,5,8,13,21,34,55,89,144, ...
or (often, in modern usage):
0,1,1,2,3,5,8,13,21,34,55,89,144, ...

By definition, the first two numbers in the Fibonacci sequence are 1 and 1, or 0 and 1, depending on the chosen starting point of the sequence, and each subsequent number is the sum of the previous two.

In mathematical terms, the sequence Fn of Fibonacci numbers is defined by the recurrence relation:

$F_n$ = $F_{n-1}$ + $F_{n-2}$,
with seed value

$F_1$ = 1; $F_2$ = 1
or
$F_0$ = 0; $F_1$ = 1.

Reference from wiki: Fibonacci number

---

## Introduction to Shiny App - Fibonacci Sequence


In this app, you can caculate any quantity of the fibonacci sequence. The system will auto-caculate the fibonacci number less or equal to the number you enter and show the final result at screen.

---

## The steps to use "Fibonacci Sequence"" app

1. Enter the number you want to caculate.
2. Click "Caculate!" button.
3. system caculate the fibonacci number less or equal you enter.
4. Show the result at the screen.


--- &interactive

## Fibonacci Sequence

<div class="row-fluid">
  <div class="span4">
    <form class="well">
      <label for="numInput">The number you input</label>
      <input id="numInput" type="text" value="1"/>
      <button id="goButton" type="button" class="btn action-button">Caculate!</button>
    </form>
  </div>
  <div class="span8">
    <h3>Fibonacci Sequence less or equal to </h3>
    <div id="inputValue" class="shiny-text-output"></div>
    <h3>is : </h3>
    <div id="prediction" class="shiny-text-output"></div>
  </div>
</div>





