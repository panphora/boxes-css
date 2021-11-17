# boxes.css — focus on writing landing page content, not CSS

## Boxes.css is the framework I've always dreamed of.

I want to launch new projects every week or two, but I need to:

1. Write content
2. Drop it into a page
3. Customize the HTML & CSS
4. Be driven crazy by HTML & CSS bugs
5. Make sure it looks good on every device

🥱

Boxes.css lets me just focus on the first two steps

1. Write content
2. Drop it into a page

✅

And takes care of the rest:

3. ~~Customize the HTML & CSS~~
4. ~~Be driven crazy by HTML & CSS bugs~~
5. ~~Make sure it looks good on every device~~

**It's all you need to design a beautiful landing page!**

## types of boxes

always use `section` elements to define boxes

Use class `.media` when wanting to include an image, animation, or video on the page
* Contains an `img`, `svg`, or `video` element
* Will maintain the media's aspect ratio (5:4) no matter what screen size the user is using (mobile / tablet / desktop)

Use class `.content` when wanting to include headings, text, or form controls on the page
* Contains `h1-h6`, `p`, `div`, `form`, `input`, `button`, `a`
* Will maintain the box's aspect ratio (5:4) on desktop devices only &mdash; on smaller screen sizes (e.g. tablet, mobile) the amount of content will determine the box's size

## what is a box

a box is a section of content (text or media) that can appear next to other sections of content

it's always responsive by default and maintains its aspect ratio where it makes sense (esp. `.media` boxes)

the goal of a box is that you define how it looks on one screen size (e.g. desktop) and it automatically will adapt to look good on every other screen size (e.g. tablet & mobile)

## headings

use classes `.h1`, `.h2`, etc. to determine size

## floating labels with inputs

In order to save room, while also being accessible, boxes.css has the concept of an input that contains its own label

When the input is clicked, its label floats slightly above it so the user can type.

Example:

![Floating label](https://remake-web-assets.s3.amazonaws.com/boxescss-floating-label.gif)

Syntax:

```html
<div class="floating-label-container">
  <input id="email" type="email" name="email" placeholder="Enter your email address">
  <label for="email">Enter your email address</label>
</div>
```

## dealing with media

always create media that has a 5:4 ration (width:height)

this will ensure that part of your media is never cut off on any screen size and will always look the same no matter what size device the user is viewing your website on

tip: since wide content works better on desktop and tablet and tall content works better on mobile, you may want to consider making one pieces of media in both formats (wide and tall) and only show the wide version on tablet and desktop and the tall one on mobile

## how to make SVGs responsive

1. make a vector image with 5:4 width to height ratio
2. export an SVG with `viewBox` attribute
3. put the SVG image in a `.media` box

[source](https://stackoverflow.com/questions/19484707/how-can-i-make-an-svg-scale-with-its-parent-container)




