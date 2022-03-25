1. Using loops take 10 inputs from user and find the average of all the numbers.

```JS
let avg = 0;
for(let i = 1; i <= 10; i++){
    let input = +prompt("Enter any number");
    avg+=input;
} 
console.log(avg/10)
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
Answer: Code doesn't executes and show error because `println` is not defined.


3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```JS
function getEvenSum(max = 10){
  let sum = 0;
  for(let i = 0; i <= max; i++){
     if( i % 2 === 0){
    sum += i;
  }
  }
  return sum
}
getEvenSum();
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```JS
function getOddSum(max = 10){
  let sum = 0;
  for(let i = 0; i <= max ; i++ ){
    if(i % 2 != 0 ){
      sum += i;
    }
  }
  return sum
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

```JS
function getProductOfDigits(num){
  if(num < 0){
    return `not a valid input`
  }else {
    let prod = 1;
    while(num > 0){
      let rem = num % 10;
      num = num - rem;
      num = num / 10;
      prod = prod * rem;
    }
      return prod;
  }
}
getProductOfDigits()
```

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); "Bigger than 5"
check(1); "Smaller than 5"
check(5); "5"
```
Answer: When conditions are true the true conditions are returning but when `5` is given as argument it will return `5` because conditions are only given for `>5` and `<5`. 

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); "You are arya";
getOutput('John'); "You are John";
getOutput(); "Who are you";
```
Answer : When conditions are true the true conditions are returning other wise in every function call  false conditions will be return.

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); "You are arya" 
                   "who are you"
getOutput('John'); "You are john" 
                   "who are you"
getOutput(); "who are you"
```
Answer :  The true argument will return true condition but along with return value, because after execution of conditions function meets to return so executes the return and conditional value.

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

```JS
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}
```
Answer : In above code function have multiple return statement and it's working because it embeded inside the opening and closing curley brackets. So if we embed return statement in individiual section with opening and closing curley brackets it will work. 

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

Answer : `for` loop takes three statements i.e. initialization, condition and iteration.`for` loop use when the condition is known.

`while` loop starts with condition and iteration rotates in body. We use `while` loop when we just have a condition and based on that we have to executes the code.

```js
//for loop

let sum = 0;
for(let i = 0; i <= 10; i++){
 sum += i/10
} 
console.log (sum)

```
```js
// while loop

let i = 0;
while( i <= 10 ){
if (i % 2 == 0){
console.log(i)
}
i++
}

```
