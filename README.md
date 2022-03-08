# Design to code challenge

The challenge was to design a website then write the code for a responsive website using HTML and CSS, trying to match the original design.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Challenge site](#challenge-site)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)
- [Web Tools Used](#web-tools-used)

## Overview

### Screenshot

![](screenshot.png)

### Challenge site

- [Live Site](https://inspiring-villani-d79eb6.netlify.app/)

## My process

### Built with

- Sketch (for the design)
- Flexbox
- CSS Grid

### What I learned

I learned that designing in Sketch or any other design tool, (Figma, Adobe XD etc.) it is then easier to code the final website because the properties for font family, font size, margin and padding have already been declared.

Instead of adding a different class to each card element, I used The `:nth-child()` CSS pseudo-class. So I could easily add a different background image to the other cards.

The `grid-gap` property is depreciated use `gap` instead. see [Acknowledgments](#acknowledgments) :point_down:

HTML
```
<div class="card">
</div>
```

CSS
```
/* Select the first card */
.card:nth-child(1) {
    background-image: url(/images/image-1.jpg);
}

/* Select the second card */
.card:nth-child(2) {
    background-image: url(/images/image-2.jpg);
}
```

For the hover state of the card, I used the `transform` CSS property, to scale the card up slightly when the user hovers over the card element.

```
.card:hover {
    transform: scale(1.02);
}
```

I used the `transition` CSS property to add a slight delay to the scale.

```
.card {
  transition: all .3s ease;
}
```

### Continued development

I would like to learn more about Figma so for the next challenge I would like to use Figma as my design tool.

I would like to become more proficient in Sass, for the next project I would like to use Sass for styling the website.

## Author

- Website - [Larrie Knights](https://larrieknights.com)
- Twitter - [@512kilobytes](https://www.twitter.com/512kilobytes)

## Acknowledgments

I referenced the following websites when I got stuck or wanted to learn more.

- [What is the difference between "screen" and "only screen" in media queries?](https://stackoverflow.com/questions/8549529/what-is-the-difference-between-screen-and-only-screen-in-media-queries)

- [Adding emojis to git github readme](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)

- [The :nth-child() CSS pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-child)

- [The transform CSS property](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)

- [The transition CSS property](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)

- The `grid-gap` in CSS grid is depreciated use `gap` instead [gap (grid-gap)](https://developer.mozilla.org/en-US/docs/Web/CSS/gap)

- [Vendor Prefix](https://developer.mozilla.org/en-US/docs/Glossary/Vendor_Prefix)

## Web Tools Used

- [autoprefixer.github.io](https://autoprefixer.github.io/) - Add vendor prefixes

- [minifier.org](https://www.minifier.org/) - Minify the CSS file

- [app.netlify.com/drop](https://app.netlify.com/drop) - Host the website

Final site is in the [_production](/_production) directory