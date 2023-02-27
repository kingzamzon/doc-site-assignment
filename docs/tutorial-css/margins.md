---
sidebar_position: 12
---

# Margins

Margins are used to create space around elements, outside of any defined borders.

## CSS Margins

The CSS `margin` properties are used to create space around elements, outside of any defined borders.

With CSS, you have full control over the margins. There are properties for setting the margin for each side of an element (top, right, bottom, and left).

## Margin - Individual Sides

CSS has properties for specifying the margin for each side of an element:

- `margin-top`
- `margin-right`
- `margin-bottom`
- `margin-left`

All the margin properties can have the following values:

- auto - the browser calculates the margin
- length - specifies a margin in px, pt, cm, etc.
- % - specifies a margin in % of the width of the containing element
- inherit - specifies that the margin should be inherited from the parent element

:::tip
Negative values are allowed.
:::

```css
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```

## Margin - Shorthand Property

To shorten the code, it is possible to specify all the margin properties in one property.

The margin property is a shorthand property for the following individual margin properties:

- margin-top
- margin-right
- margin-bottom
- margin-left
  So, here is how it works:

If the margin property has four values:

- margin: 25px 50px 75px 100px;
  - top margin is 25px
  - right margin is 50px
  - bottom margin is 75px
  - left margin is 100px

```css
p {
  margin: 25px 50px 75px 100px;
}
```

If the margin property has three values:

- margin: 25px 50px 75px;
  - top margin is 25px
  - right and left margins are 50px
  - bottom margin is 75px

```css
p {
  margin: 25px 50px 75px;
}
```

If the `margin` property has two values:

- margin: 25px 50px;
  - top and bottom margins are 25px
  - right and left margins are 50px

```css
p {
  margin: 25px 50px;
}
```

If the `margin` property has one value:

- margin: 25px;
  - all four margins are 25px

```css
p {
  margin: 25px;
}
```

## The auto Value

You can set the margin property to `auto` to horizontally center the element within its container.

The element will then take up the specified width, and the remaining space will be split equally between the left and right margins.

```css
div {
  width: 300px;
  margin: auto;
  border: 1px solid red;
}
```

## The inherit Value

This example lets the left margin of the `<p class="ex1">` element be inherited from the parent element (`<div>`):

```css
div {
  border: 1px solid red;
  margin-left: 100px;
}

p.ex1 {
  margin-left: inherit;
}
```

## All CSS Margin Properties

| Property      | Description                                                                   |
| ------------- | ----------------------------------------------------------------------------- |
| margin        | A shorthand property for setting all the margin properties in one declaration |
| margin-bottom | Sets the bottom margin of an element                                          |
| margin-left   | Sets the left margin of an element                                            |
| margin-right  | Sets the right margin of an element                                           |
| margin-top    | Sets the top margin of an element                                             |
