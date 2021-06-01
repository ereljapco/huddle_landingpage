# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot_desktop.png)
![](./screenshot_mobile.png)

### Links

- Solution URL: [Github](https://github.com/erelita/huddle_landingpage.git)
- Live Site URL: [Netlify](https://huddle-lp-erelita.netlify.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow
- [Font Awesome](https://fontawesome.com/) - For social icons
- [Google Fonts](https://fonts.google.com) - For fonts

### What I learned

First time to use semantics elements. I tried, but I don't think I did a good job. Might have overdone it a bit.

```html

<body>
    <header> 
        <section> </section>
    </header>
    <main>
        <section></section>
        <section></section>
    </main>
    <footer>
        <section></section>
        <section></section>
    </footer>
</body>

```

I tried to find ways how to do the circle around the social links and lot of them are using 2 icons and placing the circle icon behind the main icon. The circle icon that I want was only available in Pro at Font Awesome, so I tried making a class with a circle border and using it in the hyperlink tags. I'm so happy it worked!

```css
.social-icon {
    display: inline-block;
    font-size: 0.9em;
    color: var(--clr-text);
    border: 1px solid var(--clr-text);
    border-radius: 50%;
    width: 1.9em;
    height: 1.9em;
    line-height: 1.7em;
    text-align: center;
    vertical-align: middle;
    margin: 0 0.3em;
}
```

I thought that background images are automatically placed from the top left corner. Glad I worked on this project and found out that I can assign the position and size.

```css
body {
  background: var(--clr-bg) url("../images/bg-desktop.svg") left/auto 100% no-repeat scroll;
}
```

### Continued development

I wasn't able to make it responsive. I wish to learn how to make responsive layout using CSS grid. Will try to redo this in the future and make a better version.

I wanted to try using Sass, but got afraid to mess up the code I as already doing. Will definitely try it on the next challenge.

### Useful resources

I tried to look for articles and tutorials that I thought helped me, then I realized that I didn't totally understand those. Fault in my part because I was looking for something specific or what I read didn't work for the solution I was doing.

## Author

- Github - [Erelita](https://github.com/erelita/)
- Frontend Mentor - [@erelita](https://www.frontendmentor.io/profile/erelita)

## Acknowledgments

- [Dev Ed](https://www.youtube.com/c/DevEd/) - Didn't exactly help in this particular challenge, but I do want to mention him because watching his Youtube videos makes me want to code more. He makes coding fun with his tutorials. Thank you, Dev Ed!
