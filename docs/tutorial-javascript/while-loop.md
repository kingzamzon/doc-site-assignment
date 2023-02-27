---
sidebar_position: 8
---

# While Loop

Loops can execute a block of code as long as a specified condition is true.

## The While Loop

The while loop loops through a block of code as long as a specified condition is true.

```js title="Syntax"
while (condition) {
  // code block to be executed
}
```

## Example

In the following example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10:

```js
while (i < 10) {
  text += "The number is " + i;
  i++;
}
```

:::note
If you forget to increase the variable used in the condition, the loop will never end. This will crash your browser.
:::

## The Do While Loop

The `do while` loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

```js title="Syntax"
do {
  // code block to be executed
} while (condition);
```

## Example

The example below uses a `do while` loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:

```js
do {
  text += "The number is " + i;
  i++;
} while (i < 10);
```

:::note
Do not forget to increase the variable used in the condition, otherwise the loop will never end!
:::
