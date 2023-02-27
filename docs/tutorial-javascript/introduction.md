---
sidebar_position: 1
---

# Introduction

JavaScript is the world's most popular programming language.

JavaScript is the programming language of the Web.

JavaScript is easy to learn.

This tutorial will teach you JavaScript from basic to advanced.

## JavaScript Can Change HTML Content

One of many JavaScript HTML methods is getElementById().

The example below "finds" an HTML element (with id="demo"), and changes the element content (innerHTML) to "Hello JavaScript":

```js
document.getElementById("demo").innerHTML = "Hello JavaScript";
```

:::note
JavaScript accepts both double and single quotes:
:::

```js
document.getElementById("demo").innerHTML = "Hello JavaScript";
```

## JavaScript Can Change HTML Styles (CSS)

Changing the style of an HTML element, is a variant of changing an HTML attribute:

```js
document.getElementById("demo").style.fontSize = "35px";
```

## JavaScript Can Hide HTML Elements

Hiding HTML elements can be done by changing the display style:

```js
document.getElementById("demo").style.display = "none";
```

## JavaScript Can Show HTML Elements

Showing hidden HTML elements can also be done by changing the display style:

```js
document.getElementById("demo").style.display = "block";
```

:::note
JavaScript and Java are completely different languages, both in concept and design.

JavaScript was invented by Brendan Eich in 1995, and became an ECMA standard in 1997.

ECMA-262 is the official name of the standard. ECMAScript is the official name of the language.
:::
