# JavaScript
This is a review to Javascript basic knowledge. This note follows the video [here &rarr;](https://www.youtube.com/watch?v=SBmSRK3feww&list=PLEPye7A7EcQZrT3VSBb7jtxnxIfY3yyG6&index=3)

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

## 4. HTML, CSS Review, console.log, JS in HTML, comments

1. HTML  = create the content of the website
2. CSS = change the appearance
3. JavaScript = Makes it interactive

### 1. HTML Review

+ Hyper Text Markup Language  
+ Giving instruction to a computer
+ Please see html-review.html
```
<button>this is a button</button>
<p>this is a paragraph</p>
```

#### HTML syntax rules 

1. **elements**
2. HTML **tag** - opening tag and closing tag
3. **nesting** - can have elements inside elements
4. multiple space are combined into 1 space, newlines also count as spaces.
5. web page = a single page (on a website)(home page, cart page, etc. together this pages we call this website)

#### HTML atributes and its syntax rules

```
<button title="tooltip">hello</button>
<!-- titile attribute add a tooltip to the buton -->
```
1. we always put attributes on the opening tag and we add a space between the element name and the attribute to separte them.
2. Attribute name - the left side part (title)
3. Attribute value - the right side

#### class attribute

class attribute - adds a label to an element
```
  <button title="Good job" class="red-button">
    hello
  </button>
```
after we label this element, we can select it in CSS

#### HTML structure

```
<!DOCTYPE html>
<html>
  <head>
    <title>HTML CSS Review</title>
    <style>
      p {
        background-color: red;
      }
    </style>
  </head>
  <body>
    <p>this is a paragraph</p>
  </body>
</html>
```
what is benefit to following this structure?
1. there are other elements that we can use inside the head.(```<title>```element)
2. **automatically refresh our web page** when we change our code. (add "live server" extension -> settings -> choose chrome -> right click and choose open with live server)

### 2. CSS Review

*  Cascading Style Sheets
*  Change the appearance of the websites

```
<!-- change all buttons attributes -->
<style>
  button {
    background-color: red;
    color: white;
    border: none;
  }
</style>
```  

```
<!-- change the appearance of the button with label "red-button" -->
<style>
.red-button {
  background-color: red;
  color: white;
}
</style>
```
* this means we are looking for a all elements with the class red-button

#### CSS syntax rules

1. CSS selector - select which elements to change. (button{color:white}, button is CSS selector)
2. CSS styles: how to change the appearance (inside {})
3. CSS property - what we are changing (background-color).
4. CSS value - what changes the property to (red)

### 3. VSCode setup

* indents - the spaces at the front of the code in lines - read moer easier
  * be default, VSCode usally four spaces per indents
  * in HTML, CSS, JS = 2 spaces per indents (settings -> serach "tab" -> change "tab size" to 2)
* **line wraping** - set the code have approprate indents
  * if the line is too long (settings -> search "wrap" -> word wrap -> choose "on"), then it will wrap around to the next line automatically.

### 4. run JS in HTML

#### 1. use ```<script>``` 

```
<!DOCTYPE html>
<html>
  <head>
    <title>HTML CSS Review</title>
    <style>
      p {
        background-color: red;
      }
    </style>
  </head>  
  <body>
    <p>this is a paragraph</p>
    <script>
      alert('hello);
    </script>
  </body>
</html>
```
* usually put the script at the bottom of the body.
* consol = try out JavaScript code
* the code in the script element runs first when the page is loaded

#### 2. using attribute

```
  <button onclick="alert('Good Job!');">hello</button>
```
the code in the onclick attribute runs after when we click the buttons on the page.

### 5. comments in JS

Pieces of code that the computer ignores

#### 1. use "//" as oneline comment

```// this is a comment```

#### Why we use comments

1. provide more information
2. commenting out the code - don't want to run some code, don't want to delete it

#### 2. use "/**/" as multi-line comment

```
/* This 
  is a 
  comment 
 */
```

### 6. comments in HTML and CSS

1. HTML comment
``` <!-- This is a comment --> ```
2. CSS comment
``` /*This is a comment*/ ```

### 7. console.log
show the result in the console
``` console.log(2+2) ``` - the result 4 will show in console.