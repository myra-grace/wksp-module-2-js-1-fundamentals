import line from './assets/straight_line.png';
import conditional from './assets/conditional.png';
import forLoop from './assets/for_loop.png';
import whileLoop from './assets/while_loop.png';

# 2.1.5 JavaScript Control Flow

---

JavaScript executes a program from top to bottom in order.

<img src='./assets/straight_line.png' />

---

## Conditional Execution

- We will very often need a program to do things _conditionally_.

<img src='./assets/conditional.png' />

---

### The `if` Statement

- The `condition` must always evaluate to `true` for the code inside of the `{}` to actually run.
 
```js
if (condition) {
    // do something
}
```

---

```js
let number = 20;
if (number > 16) {
    console.log('Hold');
}
```

---

```js
let number = 20;
if (number > 16) {
    console.log('Hold');
} else {
    console.log('Hit me');
}
```

---

#### Exercise

Turn the following sentences into valid JavaScript `if` statements. _Use console.log() to "announce" an action._

```js
// 1. If it rains, I stay home.
let currentWeather = 'rainy';
// if (currentWeather === 'rainy') {
    //console.log ('I stay home');
//}

// 2. If I am hungry, I eat.
let hunger = true;
// if (hunger) {
    //console.log ('I eat');
//}

// 3. If it's 10pm, I go to bed. If not, I write code.
let currentHour = 22;
// if (currentHour >= 22 || currentHour <6) {
    //console.log ('I go bed'); }
    //else {
    //console.log ('I wrote code');
//}

```

## Loops

---

Here is a program that outputs all even numbers between 0 and 12.

```js
console.log(0);
console.log(2);
console.log(4);
console.log(6);
console.log(8);
console.log(10);
console.log(12);
```

This is Repetitious, but manageable...

---

Here is a program that outputs all even numbers between 0 and 1000.

```js
console.log(0);
console.log(2);
// ... on and on and on...
```

This is where loops come in!

---

### `while` Loops

<img src='./assets/while_loop.png' />

---

#### Example

```js
let number = 0;
while (number <= 12) {
    console.log(number);
    number = number + 2;
}

// let's break that down.
```

---

Let's write a function that outputs 2^10 (two to the power of ten).

```js
//let x = 1;
//let i = 1;
//while (i<=10) {
    //x=x*2;
    //i++;
//}
//console.log(x);

//SHORTER WAY USE for loop


```

---

Using `while` is MUCH better than the repetition that we had before, but it is not great.

We still need to

- define a counter
- define the condition for loop to run
- increment that counter, everytime the `while` loop runs

I wonder if there is a shorthand `for` this? 😉

---

### `for` Loops

<img src='./assets/for_loop.png' />

---

#### Example

```js
for (let number = 0; number <=12; number = number + 1) {
    if (number % 2 === 0) {
        console.log(number);
    }

}

// let's break that down.
```
let number = 0;
while (number<= 12) {
    if (number===number; number=number + 1)
    //missedd itttt
}

---

⚠️ The **ONLY** way to break out of the loop is for the condition to be `false`. ⚠️

---

- If you write a `for` loop that _always_ evaluates to `true`, your loop will continue forever.
- This is a bad thing... it will crash your environment (browser window, node env, etc.).
    - To fix it, you will need to force-quit the environment.

---

#### Exercise 1

Write a program that output all of the numbers from 0 to 25

```js
// for(let i = 0; i<= 25; i++) {
    //console.log(i);
//}

```

---

#### Exercise 2

Write a program that output all of ODD the numbers from 0 to 25

```js
// for(let i = 0; i<= 25; i++) {
    //if (i % 2 === 1) {
    //console.log(i);
    //}
//}

//OR

// for(let i = 1; i<= 25; i+=2) {
    //console.log(i);
//}

```

---

#### Exercise 3

Write a program that output all of the numbers from 0 to 25, but replaces all multipes of `5` by the phrase `five alive!`

```js
// for(let i = 0; i< 26; i++) {
    //if (i % 5 === 0 && i!== 0) {
    //console.log('Five Alive');}
    //else {
        //console.log(i);
    //}
//}

```

---