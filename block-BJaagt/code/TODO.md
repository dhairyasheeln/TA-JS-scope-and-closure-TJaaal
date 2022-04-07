Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(username); // ReferenceError: username is not defined
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the variable defined inside a block from outside.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // ReferenceError: username is not defined
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the variable defined inside a block from outside.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(username); // Arya
```

In above code we are looking for the variable named `usename`. Since username is declared using 'var' which does not work for block ,hence username can also be accessed outside the block creating global scope.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // John
```
In above code we are looking for the variable named `usename`. There is a variable named `username` in the global scope and  hence can be accessed outside the block.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // John
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); /* 0 'First'
1 'First'
2 'First'
3 'First'
4 'First'
5 'First'
6 'First'
7 'First'
8 'First'
9 'First'
*/

}
console.log(i, 'Second'); // 10 'Second'
```

In above code we are looking for the variable named `i`. There is a variable named `i` defined in for loop(block scoped) but since the variable i is declared using var keyword , it created global scope outside and hence can be accessed outside the block as well.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); /* 0 'First'
1 'First'
2 'First'
3 'First'
4 'First'
5 'First'
6 'First'
7 'First'
8 'First'
9 'First'
*/
}
console.log(i, 'Second'); // Reference Error i is not defined
```
