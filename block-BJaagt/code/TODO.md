Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // output

//In above code we are looking for the variable username. There is no variable named username in the global scope. The varible is inside a block and it is declared using const. const keyword has block scope so we can't access the varible outside

The above code will throw an error 'Reference error username is not defined'

```

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output

//In the above we are looking for a variable username and it is defined inside if block using let. The if condition will be true and it will assign the value arya to username. But we cannot access username outside if block because we are using let. 
The above code will throw an error 'Reference error username is not defined'
```

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output

//In the above we are looking for a variable username and it is defined inside if block using var. The if condition will be true and it will assign the value arya to username. 
The output of the code will be Arya
```

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output

//Here we are looking for the variable username it is defined in the global scope. first the value of username will be "John" and we are again declaring the username varible inside the if condition using var. var does not have block scope. So this will create error beacuse here we are trying to declare the same variable two times

The above code will throw syntax error username has already been created
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output

//Here we are looking for the variable username it is defined in the global scope. first the value of username will be "John" and we are again declaring the username varible inside the if condition using let let. Let is having block scope so in this case this username variable(inside if) will be different than the globla varibale.

output will be John

```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // output

//Here we are looking for the variable username which declared in two places. First it is declared as a global variable and next inside the function both using let. let is having block scope. So the output will be "John"
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output

//Here we are looking for varible i which is defined inside a for loop using var. So we can access the value of i out side for loop. So here the first output will be 

0 "First"
1 "First"
2 "First"
3 "First"
4 "First"
5 "First"
6 "First"
7 "First"
8 "First"
9 "First"
"
and the second output will be 
10 "Second"
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output

//Here we are looking for varible i which is defined inside a for loop using let. So we cannot access the i variable outside the for loop. So the first output will be

0 "First"
1 "First"
2 "First"
3 "First"
4 "First"
5 "First"
6 "First"
7 "First"
8 "First"
9 "First"

and second output will be a reference error i is not defined

```
