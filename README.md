# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](./screenshot.png)


### Links

- Solution URL: https://github.com/alessandra-casole/NFT-preview-project
- Live Site URL: https://alessandra-casole.github.io/NFT-preview-project/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

How to overlay a visible image in hover while the one below must be in transparency

```html
<h1>Some HTML code I'm proud of</h1>

  <div id="card">
    <img src="assets/img/image-equilibrium.jpg" id="card-image" alt="a illuminated cube" />
       <div id="overlay">
         <div id="view-icon">
          <img src="assets/img/icon-view.svg" alt="eye icon" id="h-icon-image"/>
         </div>
       </div>
   </div>
```
```css
.proud-of-this-css {

  #card {
    position: relative;
    background-color: hsl(178, 100%, 50%);
    border-radius: 10px;
}

  #card-image {
    width: 100%;
    border-radius: 8px;
    display: block;
    opacity: 1;
    transition: .5s ease;
}

  #overlay {
    position: absolute;
    top: 50%;
    left: 50%;
    /* width: 100%; */
    opacity: 0;
    border: 1px solid transparent;
    border-radius: 9px;
    transition: .5s ease;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    text-align: center;
}


  #card:hover #card-image {
    opacity: 0.5;
    cursor: pointer;
}

  #card:hover #overlay {
    opacity: 1;
}

```

### Continued development


### Useful resources

- https://www.w3schools.com/howto/tryit.asp?filename=tryhow_css_image_overlay_opacity - This helped me overlay the visible image in hover. I really liked this pattern and will use it going forward.


## Author

- Frontend Mentor - [@alessandra-casole](https://www.frontendmentor.io/profile/alessandra-casole)

