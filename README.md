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
An example to use [here &rarr;](https://supersimple.dev/projects/amazon/), jump tp the cart page to see the price calculation.

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
1. ```Math.round()``` - Rounding just means taking a number and moving it to the nearest **integer**. Put a number in the bracket. (we can use this to the cents frist, and then /100 to change to dollars, and it will have two decimal places).
2. ```Math.floor()``` - Rounding a number **Down** to the nearest integer.
3. ```Math.ceil()``` - Rounding a number **Up** to the nearest integer.

## 3. Strings
An example to use [here &rarr;](https://supersimple.dev/projects/amazon/checkout)   
string  = text
1. a text surronding with single quotes
2. if we add strings, they will combine together. 

### 1. Concatenation
means combine strings together.  
1. ```'some' + 'text'```, result is```'sometext'```
2. ```'some' + 'more' + 'text```, result is ```'somemoretext```

### 2. types of values
Numbers ans Strings are two different **types of values** in JavaScript. They represent different things.
1. ```typeof 2``` - check types of value, this result is ```'number'```, ```typeof 'hello'``` result is ```'string'```

### 3. Type coercion (automatic  type conversion)
```'hello' + 3``` - the result is ```'hello3'```  
If add a string and a number, JavaScript will automatically convert this number into a string  
1. ```$28.94``` is a text - ```'$' + ((2095+799)/100)``` - calculate money in cents
2. attention: ```$+20.95+7.99```, the result is ```'$20.957.99'```, it will treat as string combination.
3. *string also follow order of operations*

### 4. 3 ways to create a string
1. ```'...'``` - for example: ```'hello'```, recommond use this way by default
2. ```"..."``` - for example: ```"hello"```.  If a single quote inside the string, use double  quotes - ```"I'm learning JavaScript"``` (also can use *escape character* to solve this problem)
3. ``` `...` ``` - for example: ``` `hello` ```, we call this *template strings*, it have some features
    1. interpolation - insert value directly into a string - ``` `Items(${1+1}): $${(2095+799)/100}` ```, the result is ```'Items(2):$28.94'```, use ```${...}``` insert value directly into string  
    *This is a must easier way to insert value into a string.*
    2. multi-line string - a string have multiple lines, this feature is only available for template strings, same like have a string with ```\n```

### 5. character and escape character
character = 1 letter/number/symbol (for example, ```'hello'``` have 5 characters)
1. letter (a, b, c)
2. number (1, 2, 3)
3. symbol (!, @, #)
4. escape character (```\'```), a escape character looks like a backslash and then another character, like single quote, this combination actually counts as one character in a string. backslash do not have any meaning.For example ```'I\'m learning JavaScript'```  
    1. ```\'``` - create a single quote that is just text, it doesn't start or end the string
    2. ```\"``` - create a double quote that is just text. it doesn't start or end the string
    3. ```\n``` - new line character. it create a new line of text.