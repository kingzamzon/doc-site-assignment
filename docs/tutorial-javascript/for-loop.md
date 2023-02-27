---
sidebar_position: 9
---

# For loop

The for statement creates a loop with 3 optional expressions:

```js
for (expression 1; expression 2; expression 3) {
  // code block to be executed
}
```

**Expression 1** is executed (one time) before the execution of the code block.

**Expression 2** defines the condition for executing the code block.

**Expression 3** is executed (every time) after the code block has been executed.

```js
for (let i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}
```

From the example above, you can read:

**Expression 1** sets a variable before the loop starts (let i = 0).

**Expression 2** defines the condition for the loop to run (i must be less than 5).

**Expression 3** increases a value (i++) each time the code block in the loop has been executed.

## Expression 1

Normally you will use expression 1 to initialize the variable used in the loop (let i = 0).

This is not always the case. JavaScript doesn't care. Expression 1 is optional.

You can initiate many values in expression 1 (separated by comma):

```js
for (let i = 0, len = cars.length, text = ""; i < len; i++) {
  text += cars[i] + "<br>";
}
```

And you can omit expression 1 (like when your values are set before the loop starts):

```js
let i = 2;
let len = cars.length;
let text = "";
for (; i < len; i++) {
  text += cars[i] + "<br>";
}
```

## Expression 2

Often expression 2 is used to evaluate the condition of the initial variable.

This is not always the case. JavaScript doesn't care. Expression 2 is also optional.

If expression 2 returns true, the loop will start over again. If it returns false, the loop will end.

:::note
If you omit expression 2, you must provide a break inside the loop. Otherwise the loop will never end. This will crash your browser. Read about breaks in a later chapter of this tutorial.
:::

## Expression 3

Often expression 3 increments the value of the initial variable.

This is not always the case. JavaScript doesn't care. Expression 3 is optional.

Expression 3 can do anything like negative increment (i--), positive increment (i = i + 15), or anything else.

Expression 3 can also be omitted (like when you increment your values inside the loop):

```js
let i = 0;
let len = cars.length;
let text = "";
for (; i < len; ) {
  text += cars[i] + "<br>";
  i++;
}
```

## Loop Scope

Using `var` in a loop:

```js
var i = 5;

for (var i = 0; i < 10; i++) {
  // some code
}

// Here i is 10
```

Using `let` in a loop:

```js
let i = 5;

for (let i = 0; i < 10; i++) {
  // some code
}

// Here i is 5
```

In the first example, using `var`, the variable declared in the loop redeclares the variable outside the loop.

In the second example, using `let`, the variable declared in the loop does not redeclare the variable outside the loop.

When `let` is used to declare the i variable in a loop, the i variable will only be visible within the loop.

Comparing While and For
If you have read the previous chapter, about the while loop, you will discover that a while loop is much the same as a for loop, with statement 1 and statement 3 omitted.

The loop in this example uses a `for` loop to collect the car names from the cars array:

```js
const cars = ["BMW", "Volvo", "Saab", "Ford"];
let i = 0;
let text = "";

for (; cars[i]; ) {
  text += cars[i];
  i++;
}
```

The loop in this example uses a `while` loop to collect the car names from the cars array:

```js
const cars = ["BMW", "Volvo", "Saab", "Ford"];
let i = 0;
let text = "";

while (cars[i]) {
  text += cars[i];
  i++;
}
```
