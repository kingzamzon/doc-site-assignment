---
sidebar_position: 9
---

# Images

Images can improve the design and the appearance of a web page.

```html
<img src="pic_trulli.jpg" alt="Italian Trulli" />
```

## HTML Images Syntax

The HTML `<img>` tag is used to embed an image in a web page.

Images are not technically inserted into a web page; images are linked to web pages. The `<img>` tag creates a holding space for the referenced image.

The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.

The `<img>` tag has two required attributes:

- src - Specifies the path to the image
- alt - Specifies an alternate text for the image

```html
<img src="url" alt="alternatetext" />
```

## The src Attribute

The required `src` attribute specifies the path (URL) to the image.

Note: When a web page loads, it is the browser, at that moment, that gets the image from a web server and inserts it into the page. Therefore, make sure that the image actually stays in the same spot in relation to the web page, otherwise your visitors will get a broken link icon. The broken link icon and the alt text are shown if the browser cannot find the image.

```html
<img src="img_chania.jpg" alt="Flowers in Chania" />
```

## The alt Attribute

The required `alt` attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

The value of the `alt` attribute should describe the image:

```html
<img src="img_chania.jpg" alt="Flowers in Chania" />
```

If a browser cannot find an image, it will display the value of the alt attribute:

```html
<img src="wrongname.gif" alt="Flowers in Chania" />
```

:::tip

A screen reader is a software program that reads the HTML code, and allows the user to "listen" to the content. Screen readers are useful for people who are visually impaired or learning disabled.

:::

## Image Size - Width and Height

You can use the style attribute to specify the width and height of an image.

```html
<img
  src="img_girl.jpg"
  alt="Girl in a jacket"
  style="width:500px;height:600px;"
/>
```

Alternatively, you can use the width and height attributes:

```html
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600" />
```

The width and height attributes always define the width and height of the image in pixels.

:::note

Always specify the width and height of an image. If width and height are not specified, the web page might flicker while the image loads.

:::

## Width and Height, or Style?

The width, height, and style attributes are all valid in HTML.

However, we suggest using the style attribute. It prevents styles sheets from changing the size of images:

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      img {
        width: 100%;
      }
    </style>
  </head>
  <body>
    <img src="html5.gif" alt="HTML5 Icon" width="128" height="128" />

    <img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;" />
  </body>
</html>
```

## Images in Another Folder

If you have your images in a sub-folder, you must include the folder name in the src attribute:

```html
<img
  src="/images/html5.gif"
  alt="HTML5 Icon"
  style="width:128px;height:128px;"
/>
```

## Images on Another Server/Website

Some web sites point to an image on another server.

To point to an image on another server, you must specify an absolute (full) URL in the src attribute:

```html
<img
  src="https://www.w3schools.com/images/w3schools_green.jpg"
  alt="W3Schools.com"
/>
```

:::note

External images might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; they can suddenly be removed or changed.

:::

## Animated Images

HTML allows animated GIFs:

```html
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;" />
```

## Image as a Link

To use an image as a link, put the `<img>` tag inside the `<a>` tag:

```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;" />
</a>
```

## Image Floating

Use the CSS float property to let the image float to the right or to the left of a text:

```html
<p>
  <img
    src="smiley.gif"
    alt="Smiley face"
    style="float:right;width:42px;height:42px;"
  />
  The image will float to the right of the text.
</p>

<p>
  <img
    src="smiley.gif"
    alt="Smiley face"
    style="float:left;width:42px;height:42px;"
  />
  The image will float to the left of the text.
</p>
```

## Common Image Formats

Here are the most common image file types, which are supported in all browsers (Chrome, Edge, Firefox, Safari, Opera):

| Abbreviation | File Format                           | File Extension                   |
| ------------ | ------------------------------------- | -------------------------------- |
| APNG         | Animated Portable Network Graphics    | .apng                            |
| GIF          | Graphics Interchange Format           | .gif                             |
| ICO          | Microsoft Icon                        | .ico, .cur                       |
| JPEG         | Joint Photographic Expert Group image | .jpg, .jpeg, .jfif, .pjpeg, .pjp |
| PNG          | Portable Network Graphics             | .png                             |
| SVG          | Scalable Vector Graphics              | .svg                             |
