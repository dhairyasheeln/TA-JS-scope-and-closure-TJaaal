1. What does thread of execution means in JavaScript?
Thread of execution is how javascript executes the code line by line.

2. Where the JavaScript code gets executed?
Javascript executes the code in Global Execution context.

3. What does context means in Global Execution Context?
Context is the environment in which code  gets executed.


4. When do you create a global execution context.
Global execution context get created only once for each program.

5. Execution context consists of what all things?
Execution context consists of two main things. 1)Memory -  to store the data 2)Function Execution context: Where the execution happens

6. What are the different types of execution context?
1)Global Execution Context 2)Function Execution Context

7. When global and function execution context gets created?
Global execution context gets created only once at the start of the program by JS engine and Function execution context gets created everytime a function is executed in GEC

8. Function execution gets created during function execution or while declaring a function.
Function execution gets created while executing the function

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)