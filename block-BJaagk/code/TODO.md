1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

let per=function (marks,total){
  return (marks * 100) / total;
}

let perArrow=(marks,total)=>{
  return (marks * 100) / total;
}

let perArrow=(marks,total)=>(marks * 100) / total;


// Your code goes here
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
//Function Declaration


```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
//Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
//Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

//Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;

//Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
Since function is considered as object in javascript ans as object is an expression ,function definition is also considered as an expression in javascript.
```js
let display=function (name)=>return name;
```

4. Why is a function call an expression in JavaScript?
A function call resolves to a value when called and hence it is an expression.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b; 
}

let five = add(2, 3); // Valid , beacuse it is a function call
five = add; // Valid
five = five(10, 11); // Valid
five = function () {
  return 'Hello';
}; // Valid
```

6. What is the difference between function definition and function call? Explain with an example.
Function definition is a collection of steps which will be performed for a particular fucntion whereas function call is executing the function steps which are defined in a function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

percentage(88,100);
```

7. What is the similarities between function definition and function call?
Both function definition and function call are expression and can be assigned to a variable


8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid
```

9. What is higher order function explain with an example.
When a function that accepts another function as an arguement or return a function is called higher order function.

10. Explain what is callback function. Why you can pass a function inside a function?
When we pass a function to another function , the function that is passed is known as callback function.
We can pass a function inside a function because function only accepts expressions as an arguement and since function is an object in JS and object is an expression so function is also an expression.