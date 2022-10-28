# Frontend Mentor - Stats preview card component solution

This is my solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62).  

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshotfementor.PNG)


### Links

- Solution URL: [Github URL](https://github.com/Mikerniker/Frontend-Mentor-Challenges/tree/main/005%20Stats%20Preview%20Card)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

- Reviewed css line-height property to adjust the height of the paragraph.
- Tried working on media queries, but I still find it confusing but was able to workout the responsiveness for smaller screens.
- The image did not fit the div initially so I had to add `vertical-align: top;`
- Tried an overcomplicated color code for the purple image overlay but found a simpler option:
- Mental Note: I originally used this code:
```
.card-image {
    max-width: 50%;
    position: relative; 
}

.card-image:before {
    content: "";
    display: block;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: rgba(170, 92, 219, 0.5);
}
```
- I changed it to:
```
.card-image {
    position: relative;   
    width: 90%;
    height: auto; 
    background-color: rgba(170, 92, 219, 0.5);  /*added*/
}

.hero-image {  
    width: 100%;
    height: 100%; 
    border-radius: 0 10px 10px 0;
    bottom: 0;
    vertical-align: top;
    mix-blend-mode: soft-light; /*added*/
}
```
- Learned about mix-blend-mode to add color to an image.

### Useful resources

- [Image Tint with CSS](https://www.impressivewebs.com/image-tint-blend-css/) - This was the initial source that I used to add purple tint to the image.
- [Mix-Blend-Mode](https://www.w3schools.com/cssref/pr_mix-blend-mode.php) - This was the final option I used to help me add purple tint to the image.


## Author

- Website - [Mik](https://mikerniker.github.io/Project_Website/)
- Frontend Mentor - [@Mikerniker](https://www.frontendmentor.io/profile/Mikerniker)
