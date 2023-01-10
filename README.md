# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](screenshots/Screenshot%20Desktop.png)
![](screenshots/Screenshot%20Mobile.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://gauravkumawat2002.github.io/stats-preview-card-component-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

Through this challenge, I've learnt to change images on the basis of screen-size without using any external JavaScript or CSS Media Query. I've used the <picture> tag to use different images at different screen-sizes.
I've also learnt about CSS property

```CSS
mix-blend-mode
```

to blend an image with background-color of it's parent div.

```html
<div class="container__img">
  <picture>
    <source
      media="(min-width: 768px)"
      srcset="images/image-header-desktop.jpg"
    />
    <source
      media="(min-width: 320px)"
      srcset="images/image-header-mobile.jpg"
    />
    <img src="images/image-header-mobile.jpg" alt="header-image" />
  </picture>
</div>
```

```css
.container__img {
  background-color: var(--accent);
}

.container__img > picture,
.container__img > picture > img {
  opacity: 0.9;
  mix-blend-mode: multiply;
}
```

### Continued development

I'm further looking to sharpen my skills in making responsive layouts, writing efficient code.

## Author

- Frontend Mentor - [@yGauravKumawat2002](https://www.frontendmentor.io/profile/GauravKumawat2002)
