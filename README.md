# boxes.css 

## Focus on writing landing page content, not CSS

### types of boxes

always use `section` elements to define boxes

Use class `.media`
Use class `.content`

### what is a box

a box is a section of content (text or media) that can appear next to other sections of content

it's always responsive by default and maintains its aspect ratio where it makes sense (esp. `.media` boxes)

the goal of a box is that you define how it looks on one screen size (e.g. desktop) and it automatically will adapt to look good on every other screen size (e.g. tablet & mobile)

### floating labels with inputs

```html
  <div class="floating-label-container">
    <input id="email" type="email" name="email" placeholder="Enter your email address">
    <label for="email">Enter your email address</label>
  </div>
```

### how to make SVGs responsive

1. make a vector image with 5:4 width to height ratio
2. export an SVG with `viewBox` attribute
3. put the SVG image in a `.media` box

[source](https://stackoverflow.com/questions/19484707/how-can-i-make-an-svg-scale-with-its-parent-container)


### known issues

* Images inside `.media` boxes sometimes don't expand to fill the entire box — there's a slight gap (example)