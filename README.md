# JavaScript
This is a review to Javascript basic knowledge. This note is following the video [here &rarr;](https://www.youtube.com/watch?v=SBmSRK3feww&list=PLEPye7A7EcQZrT3VSBb7jtxnxIfY3yyG6&index=3)

## 1. JavasScript Basic

### 1. What is JavaScript?
1. A technology that we use to create websites. (A website is like youtube.com or amazon.com, is how we access website on our computer). 
2. Giving instructions to a computer(code), then the computer follows our instructions(running the code)

### 2. 3 technonolgies we use to create websites
1. HTML - create the content of the website. it creates all the buttons, the text, and the images.
2. CSS - change the appearance of the websites. Using CSS can make a website looks nice.
3. JavaScript - makes the website interactive.

### 3. Terminology
1. code - the instructions we give to the computer.
2. running the code - Press enter and the computer follows our instructions
3. Programming Languages - There are many different languages we can use to write code called programming languages. It is similiar to human languages (but for code), like JavaScript, Python, Java. 

### 4. What we can do with JavaScript code?
1. ```alert('Hello, World!');``` - create a popup window on the webste. (can do this in the console)
2. Math - ```2+2```
3. ```document.body.innerHTMl = 'hello';``` - It removes everything on the page and replaces with the text "hello" (We use JS to modify the webpage) (Take Care, *JavaScript is case-sensitive* )   
...

### 6. Syntax
1. rules that we hace to follow when using a programming language like JS
2. similar to English grammar (don't need follow the grammar perfectly, people still can understand)
3. in programming, we have to follow the rules of syntax exactly, otherwise computer can't understand

## 2. Numbers and Math
An example to use [here &rarr;](https://supersimple.dev/projects/amazon/) 

In a console:   
1. ```2 + 2``` - press enter and show the **adding** result is 4
2. ```10 - 3``` - press entern and the computer **subtrats** these two numbers and shows 7
3. ```10 * 3``` - **multiplying**
4. ```10 / 2``` - **dividing**, using forward slash

### 1. Syntax Rules for numbers and math
1. write it out like normal math
2. can do math with **more than two** numbers - ```2 + 2 * 2```
3. can handle **decimal numbers** - ```2.2 + 2.2```

### 2. Order of Operations (also called operator precedence)
1. Adding, substracting, Multiplying, Dividing are called operations (operators in the middle).
2. Multiply and divide are done first, add and subtract and done after.
3. Use ```()``` to control the calculation's priority.

### 3. Calculations using floats can be inaccurate
#### 1. Terminologies
1. **Integers** - ```1, 2, 3```
2. **Floating point numbers** (floats) - ```2.2, 2.5```. *Calculations with floats are somtimes inaccurate*, because computers can't store some floats properly.
#### 2. How to avoid produce a wrong results when calculate floats.
When working with money, **Do the calcualtion in cents, then convert back to dollars**. $20.95 + $7.99, we use ```(2095 + 799) / 100``` 

### 4. How to round a number
1. Rounding just means taking a number and moving it to the nearest **integer**.
2. Use ```Math.round()```, put a number in the bracket. (we can use this to the cents frist, and then /100 to change to dollars, and it will have two decimal places).