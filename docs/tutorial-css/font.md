---
sidebar_position: 6
---

# Font

Choosing the right font for your website is important!

## Font Selection is Important

Choosing the right font has a huge impact on how the readers experience a website.

The right font can create a strong identity for your brand.

Using a font that is easy to read is important. The font adds value to your text. It is also important to choose the correct color and text size for the font.

## Generic Font Families

In CSS there are five generic font families:

1. _Serif_ fonts have a small stroke at the edges of each letter. They create a sense of formality and elegance.
2. _Sans-serif_ fonts have clean lines (no small strokes attached). They create a modern and minimalistic look.
3. _Monospace_ fonts - here all the letters have the same fixed width. They create a mechanical look.
4. _Cursive_ fonts imitate human handwriting.
5. _Fantasy_ fonts are decorative/playful fonts.
   All the different font names belong to one of the generic font families.

## Some Font Examples

| Generic Font Family | Examples of Font Names |
| ------------------- | ---------------------- |
| Serif               | Times New Roman        |
|                     | Georgia                |
|                     | Garamond               |
| Sans-serif          | Arial                  |
|                     | Verdana                |
|                     | Helvetica              |
| Monospace           | Courier New            |
|                     | Lucida Console         |
|                     | Monaco                 |
| Cursive             | Brush Script MT        |
|                     | Lucida Handwriting     |
| Fantasy             | Copperplate            |
|                     | Papyrus                |

## The CSS font-family Property

In CSS, we use the `font-family` property to specify the font of a text.

:::note
If the font name is more than one word, it must be in quotation marks, like: "Times New Roman".
:::

The `font-family` property should hold several font names as a "fallback" system, to ensure maximum compatibility between browsers/operating systems. Start with the font you want, and end with a generic family (to let the browser pick a similar font in the generic family, if no other fonts are available).

```css
.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}
```
