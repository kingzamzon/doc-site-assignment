---
sidebar_position: 8
---

# Comments

HTML comments are not displayed in the browser, but they can help document your HTML source code.

## HTML Comment Tag

You can add comments to your HTML source by using the following syntax:

```html
<!-- Write your comments here -->
```

Notice that there is an exclamation point (!) in the start tag, but not in the end tag.

:::note

Comments are not displayed by the browser, but they can help document your HTML source code.

:::

## Add Comments

With comments you can place notifications and reminders in your HTML code:

```html
<!-- This is a comment -->

<p>This is a paragraph.</p>

<!-- Remember to add more information here -->
```

## Hide Content

Comments can be used to hide content.

This can be helpful if you hide content temporarily:

```html
<p>This is a paragraph.</p>

<!-- <p>This is another paragraph </p> -->

<p>This is a paragraph too.</p>
```

You can also hide more than one line. Everything between the `<!-- and the -->` will be hidden from the display.

```html
<p>This is a paragraph.</p>
<!--
<p>Look at this cool image:</p>
<img border="0" src="pic_trulli.jpg" alt="Trulli">
-->
<p>This is a paragraph too.</p>
```

Comments are also great for debugging HTML, because you can comment out HTML lines of code, one at a time, to search for errors.

## Hide Inline Content

Comments can be used to hide parts in the middle of the HTML code.

```html
<p>
  This
  <!-- great text -->
  is a paragraph.
</p>
```
