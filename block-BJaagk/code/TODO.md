1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

//
 let percentage = function(marks, total) {
  return (marks * 100) / total;
}

let percentage = (marks, total) => (marks * 100) / total;

let precentage = function percentage(marks, total) {
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer

//function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

//function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

//funcxtion expression

```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

//function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;

function expression

```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

//Because functions are objects in Javascript. 
let sum = (num1, num2)  => num + num2;

4. Why is a function call an expression in JavaScript?

//Because function in javascript is an object. Calling a function will return a value or undefined this we can assign to a variable or some thing else

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
} 

let five = add(2, 3); // valid we can use function call as an expression
five = add; // valid here add is a function reference function is a object in js so we can assign it to variable
five = five(10, 11); // valid  we can use function call as an expression
five = function () {
  return 'Hello';
}; // valid function can be assigned to avariable in js
```

6. What is the difference between function definition and function call? Explain with an example.
//Function call means we are executing the function and function definition means we are declaring the function. Function call will have function and paranthesis and arguments. Function definition will have function keyword, name and body.

//function definition 

function add(num1, num2) {
  return num1 + num2;
}

//function call

add(2, 3);

7. What is the similarities between function definition and function call?

//both contains function name and both are expressions. 
function definition is an expression (function is a object in js)
function call is an expressions (always returns a value)

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid  because functions in js are objects

here we are first defining a hello function and in second we are assigning the value "Sam" to user key in hello object
```

9. What is higher order function explain with an example.

//Function that accepts or returns function is called higher order function

let numbers = [1, 2, 3, 4, 5, 6];

let evenNumbers = numbers.filter((elm) => {
  return elm % 2 === 0;
});

here we are passing a callback function as argument to filter method that will return the even numbers from the array

10. Explain what is callback function. Why you can pass a function inside a function?

//Function that is passed as argument to another function is called a callback function. We can pass a function inside another function because function in js are expressions we can pass expressions as arguments to a function