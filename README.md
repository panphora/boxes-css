# boxes.css 

## Focus on writing landing page content, not CSS

### types of boxes

Use class `.media`
Use class `.content`

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