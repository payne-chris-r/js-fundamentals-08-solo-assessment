![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Assessment for JavaScript Fundamentals

You have 20 minutes

## Instructions

Fork, clone, and npm install.

Follow the prompts below and complete each question.  You may use any resource, other than someone else in the classroom, to help you complete this assessment.

You should save your answers in this README.md file.

# Question 1

```js
var a = 2;
var b = 3;
a = b;
```

After this code executes, what are the values of a and b? Please explain your answer.

a and b both equal 3. During the code, a is set equal to 2, and b set equal to 3. A is then set equal to/takes the value of b (which has a value of 3). Therefore a and b both equal 3.

## Question 2

```js
var c = 5;
var d = 2;
c = c + d;
```

After this code executes, what is the value of c?  Please explain what the last line of this program `c = c + d;` means.

c = 7
c = c + d means c should take the value of c + d combined. It would be the same as setting c = (5 + 2).

## Question 3

```js
var x = 4;
var y = 3;
x = y;
y = 10;
```

After this code executes, what are the values of x and y?  Please explain your answer.

x = 3
y = 10
To start, x is set equal to 4, and y to 3. Line 3 states x should take the value stored in y (3). At this point they are both 3. Line 4 states y should take the value 10 (replacing 3).

## Question 4

```js
var weather;
weather = "sunny";
weather === "sunny";
```

What are the values of these expressions?  Explain your answers.

Line 1: undefined
Line 2: 'sunny'
Line 3: true

The first line instantiates the variable 'weather'. While this creates the variable in memory, the expression evaluates to 'undefined.'
The second line sets the value of weather equal to the string 'sunny'. The value of this expression is 'sunny'.
The third line is an equal to test asking if what is stored in the variable 'weather' is equal to the string 'sunny'. Since this is the case, the expression evaluates to true.

## Question 5

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi >= 3) {
  console.log("sushi is delicious");
}

if (x > 0) {
  console.log("sushi is tasty");
}
```

Imagine that you take the code from this question, save it to a file called `food.js`, and run `node food.js` in your Terminal.

What would be the output? Explain your answer.

Nothing. howMuchILikeSushi is set to 2, and therefore the first if() statement is false. howMuchIlikeSushi is !>=3, so this block of code doesn't execute. Likewise, below, there is no value (that we can see) set to x. So as far as I can tell x is undefined. Therefore, this block of code won't run because x !> 0, it's undefined.

## Question 6

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi > 0) {
  console.log("sushi is tasty");
} else if (x >= 3) {
  console.log("sushi is delicious");
} else {
  console.log("I don't like sushi");
}
```

Imagine that you take the code from this question, save it to a file called `sushi.js`, and run `node sushi.js` in your Terminal.

What would be the output? Explain your answer.

"Sushi is tasty"
Since hMILS is > 0, it will move into that block of code and print to the console. There is no way for it to print "sushi is delicious" because in order for x >= 3 it has to be > 0. It will never get to the else if piece. If you put a negative number in, you will get "I don't like sushi".

## Question 7

```js
//We'll learn about require later in the course
var ask = require('./ask.js');

var answer = 'not empty';

while (answer !== '' && answer !== 'SeCrEt') {
  answer = ask("Guess my secret? ");
}
```

Imagine that you take the code from this question, save it to a file called `name.js`, and run `node name.js` in your Terminal.

What would you have to type to exit the while loop?  Explain your answer.

Error out without ask.js in the same directory (unless this is what 'require' does). If you have the necessary accompanying code. It will print "Guess my secret? " to the console and wait for a prompt from the user.  The conditions of the while loop are that answer is not equal to an empty string/'' (which it is not, so this evaluates to true) AND that it not equal the string 'SeCrEt' (which it does not--it equals 'not empty', which also evaluates to true. The program will continue to print "Guess my secret? " after each answer to the console and wait for a prompt from the user until the user types the string 'SeCrEt'.

---

Commit and push your changes.

Submit a pull request.
