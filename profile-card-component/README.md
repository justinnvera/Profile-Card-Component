# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Profile card component solution](#frontend-mentor---profile-card-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
    - [Useful resources](#useful-resources)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![](screenshot.jpg)

### Links

- Solution URL: [Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ/hub/profile-card-component-css-flexbox-and-grid-B-KtvrgRLC)
- Live Site URL: [Vercel](https://profile-card-component-psi-wine.vercel.app)

### Built with

- Semantic HTML5 markup
- CSS Flexbox
- CSS Grid

### What I learned

I learned how to use the CSS Grid effectively and how to position the background images for the page which was the biggest challenge. I also learned how to effectively use the CSS `position: relative` and `position: absolute` properties to align the `.profile-image` element in the between the  `.top` and `.middle` containers. I also learned how to manipulate multiple `background-images`.

Background image alignment below: 
```css
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 100%;
    background-color: hsl(185, 75%, 39%);
    font-family: 'Kumbh Sans', sans-serif;
    /* The background positioning styles are from https://github.com/mohammedlahboub/Profile-card-component/blob/main/css/styles.css */
    background-image: url(../images/bg-pattern-top.svg),url(../images/bg-pattern-bottom.svg);
    background-repeat: no-repeat,no-repeat;
    background-position: right 60vw bottom 39vh, left 60vw top 39vh;
    /* All credits go to @mohammedlahboub | https://www.frontendmentor.io/solutions/solution-for-profile-card-component-with-my-custom-theme-nK0RrhZBbi */
}
```

Profile image alignment below:
```css
/* ? Middle ? */
.middle {
    grid-area: middle;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    position: relative;
}
.middle .profile-image {
    position: absolute;
    top: -100px;
    border-radius: 50%;
    border: 4px white solid;
}
```
### Continued development

I want to keep learning how to use the CSS `position: relative` and `position: absolute` together with aligning elements. 

### Useful resources

- [Github](https://github.com/mohammedlahboub/Profile-card-component/blob/main/css/styles.css) - This is where I copy + pasted the styles on how to align the background images.
- [Frontend Mentor Solution](https://www.frontendmentor.io/solutions/solution-for-profile-card-component-with-my-custom-theme-nK0RrhZBbi) - All credits go to @mohammedlahboub
- 
## Author

- Website - [Justin Vera](https://www.justinvera.com)
- Frontend Mentor - [@justinnvera](https://www.frontendmentor.io/profile/justinnvera)

## Acknowledgments

The background images alignment styles are all @mohammedlahboub's work which you can find under [Useful Resources](#Useful-resources).
