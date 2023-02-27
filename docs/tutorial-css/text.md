---
sidebar_position: 7
---

# Text

CSS has a lot of properties for formatting text.

## Text Color

The color property is used to set the color of the text. The color is specified by:

- a color name - like "red"
- a HEX value - like "#ff0000"
- an RGB value - like "rgb(255,0,0)"

The default text color for a page is defined in the body selector.

```css
body {
  color: blue;
}

h1 {
  color: green;
}
```

## Text Color and Background Color

In this example, we define both the `background-color` property and the `color` property:

```css
body {
  background-color: lightgrey;
  color: blue;
}

h1 {
  background-color: black;
  color: white;
}

div {
  background-color: blue;
  color: white;
}
```

:::important

High contrast is very important for people with vision problems. So, always ensure that the contrast between the text color and the background color (or background image) is good!

:::
