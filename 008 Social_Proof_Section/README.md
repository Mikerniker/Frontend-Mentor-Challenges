#IN PROGRESS

# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). 

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


**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](./screenshot.jpg)



### Links

- Solution URL: [Github URL](https://your-solution-url.com)
- Live Site URL: [Live Site](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned

How to repeat an image within a div using background-repeat: repeat-x

```
.star-ratings {
  background: url('./images/icon-star.svg');
  width:85px;
  height:20px;
  background-repeat: repeat-x;
}
```



Had a hard time figuring out how to add a gap in the customer review section. Part of the difficulty was initially adding a dark background color in the .customer-review-section, which affected my view of the gap, as it colored over the whole section, but this was fixed after moving the background-color to the .customer class. Same with the border radius

final code

```
.customer-review-section {
  color: hsl(0, 0%, 100%);
  display: flex;
  justify-content: center;
  column-gap: 10px;
}

.customers {
  background-color: hsl(300, 43%, 22%);
  border-radius: 10px;
}
```
Learned and reviewed the "align-self" property in css to move the ratings section around
final code:
```
.first-rating {
  align-self: end;
}

.second-rating {
  align-self: center;
}

.third-rating {
  align-self: start;
}
```

- Was stuck for a while on how to change the height of the customer review section. I was finally able to change it by adjusting the margins:
```
.irene {
  margin: 1rem 0rem -1rem 0rem;
}

.anne {
  margin: 2rem 0rem -2rem 0rem;
}
```

- Mental Note: Sometimes I forget to simply use ```text-align: center``` to align text as I sometimes confuse it with justify-content or align-items. 

### Continued development



### Useful resources

- [Background-repeat: repeat-x](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat) - This helped me
- [Inline-flex vs Inline-block](https://www.geeksforgeeks.org/what-is-the-difference-between-inline-flex-and-inline-block-in-css/) - This is an 

- [Align-self](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Aligning_Items_in_a_Flex_Container) - Helpful reference on align self, in the section "Changing the main axis" 

## Author

- Website - [Mik](https://mikerniker.github.io/Project_Website/)
- Frontend Mentor - [@Mikerniker](https://www.frontendmentor.io/profile/Mikerniker)
