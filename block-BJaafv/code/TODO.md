1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
<!-- first answer -->

With return keyword we can store our value in a variable and when we call this variable our output will shown.

<!-- second answer -->

With console our ouput will show but with undefined and we can't store the value in any variable. If we store it using variable it will return undefined.


2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

Answer: If we store the returned value of first in a variable `first`, and when we call this variable it will show the final output. While with `second` variable it will return undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

Answer: Output of `sum` will be `36` because with function name we are taking only two parameters/placeholders i.e. `a, b` so only two value will add, third value not added because there is no placeholder for third value.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

Answer: Yes, we can store the first `sum` function in `add` variable because here we are using return keyword in function body and with return keyword we can store our function in a variable.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```JS
 function sayHello(name) {
   return name;
 }
 sayHello("Hello Arya");
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
Answer : Output of above given function is `Hello John`. Here we are defining variable outside the function, so when we call the function the return keyword firstly look inside the function for relevant variable and if not found then look outside the function. 

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName);  `John`

showMessage();  `Hello John`

alert(userName);  `John`
```

8. What is a Anonymous Function give example of three functions.

Answer : When we write function without the function name and store the function in a variable it called anonymous function.

examples of three function.

```JS
//function declaration

function addNumbers(numA, numB) {
  return numA + numB;
}
addNumbers(4, 8)

//function expression / anonymous function expression

let addNumbers = function(numA, numB) {
  return numA + numB;
}
addNumbers(10, 30)

// arrow function

let addNumbers = (numA, numB) => {
  return numA + numB;
} 
addNumbers(20, 40)

```

9. Can function declaration be a Anonymous Function? Explain

Answer : No, function declaration can't be an anonymous function, beacuse without function name we are not able to call the particular function and function statements require a function name.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

Answer : userName , addNumbers , showMessage , sayHello , getFullName

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
