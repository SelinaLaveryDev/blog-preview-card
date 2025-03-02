# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Your challenge is to build out this blog preview card and get it looking as close to the design as possible.

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![](https://sel-dev-bucket.s3.us-east-1.amazonaws.com/Frontend-mentor/blog-preview-2.png)

### Links

View my solution [here](https://selinalaverydev.github.io/blog-preview-card/)

## My process

- Revised the instructions and design documents
- Defined CSS variables for text presets set out in the figma file
- Wrote up semantic HTML
- Used flexbox for responsiveness

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

I learned how quickly Figma can help define CSS variables for text presets.

```css
:root {
  /* colours */
  --yellow: #f4d04e;
  --gray-950: #111111;
  --gray-500: #6b6b6b;
  --white: #ffffff;

  /* typography */
  /* typography */
  --figtree-extra-bold: "FigtreeExtraBold";
  --figtree-medium: "FigtreeMedium";

  --text-24: 2.4rem;
  --text-16: 1.6rem;
  --text-14: 1.4rem;

  --line-height-150: 150%;

  --letter-spacing-0: 0;

  --spacing-300: 2.4rem;
  --spacing-150: 1.2rem;
  --spacing-100: 0.8rem;
  --spacing-50: 0.4rem;
}
```

Created classes using the variables to match with the Figma design styles

```classes
.text-preset-1 {
  font-family: var(--figtree-extra-bold);
  font-size: var(--text-24);
  line-height: var(--line-height-150);
  letter-spacing: var(--letter-spacing-0);
}

.text-preset-2 {
  font-family: var(--figtree-medium);
  font-size: var(--text-16);
  line-height: var(--line-height-150);
  letter-spacing: var(--letter-spacing-0);
  color: var(--gray-500);
}

.text-preset-3 {
  font-family: var(--figtree-medium);
  font-size: var(--text-14);
  line-height: var(--line-height-150);
  letter-spacing: var(--letter-spacing-0);
}

.text-preset-3-bold {
  font-family: var(--figtree-extra-bold);
  font-size: var(--text-14);
  line-height: var(--line-height-150);
  letter-spacing: var(--letter-spacing-0);
}
```

Here, I used @font-face to use the font file in assets:

```@font-face
      @font-face {
  font-family: "FigtreeExtraBold";
  src: url("./assets/fonts/static/Figtree-ExtraBold.ttf") format("opentype");
}

@font-face {
  font-family: "FigtreeMedium";
  src: url("./assets/fonts/static/Figtree-Medium.ttf") format("opentype");
}
```

## Author

- [My Portfolio Website](https://selinalaverydev.github.io/selina-dev-portfolio/)
- [My Frontend Mentor Profile](https://www.frontendmentor.io/profile/SelinaLaveryDev)
- [My Github Profile](https://github.com/SelinaLaveryDev)
