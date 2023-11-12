# Developer's note

This is by no means a perfect solution. There are a lot of layout bugs I tried to fix but didn't have enough skills as of now. Most of the standard layout will work - Desktop, Tablet and Mobile.

# Frontend Mentor - Space tourism website solution

This is a solution to the [Space tourism website challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/space-tourism-multipage-website-gRWj1URZ3). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
  - [screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for each of the website's pages depending on their device's screen size
- See hover states for all interactive elements on the page
- View each page and be able to toggle between the tabs to see new information

### Links

- Solution URL: [Solution](https://www.frontendmentor.io/solutions/solution-space-tourism-website-qU5e3Aju97)
- Live Site URL: [Github](https://ahmed5xp.github.io/space-tourism/)


### screenshot 
![](CAPTURE.PNG)
## My process

### Built with

- Semantic HTML5 markup
- CSS, Flexbox and Grid
- JavaScript

### What I learned

First thing that come to mind is navbar and the styling of it. I didn't know that I can do glassmorphism with it - background blur and stuffs.

```html
<nav>
  <ul class="primary-navigation underline-indicators flex">
    <li class="active">
      <a class="text-white uppercase letter-spacing-2" href="#"
        ><span>00</span>Active</a
      >
    </li>
    <li>
      <a class="text-white uppercase letter-spacing-2" href="#"
        ><span>01</span>Hovered</a
      >
    </li>
    <li>
      <a class="text-white uppercase letter-spacing-2" href="#"
        ><span>02</span>Idle</a
      >
    </li>
  </ul>
</nav>
```

Another thing I learned in this project is using Custom Properties and utility classes, it's like making a library of your own.

```css
.bg-dark { background-color: hsl( var(--clr-dark) );}
.bg-accent { background-color: hsl( var(--clr-light) );}
.bg-white { background-color: hsl( var(--clr-white) );}

.text-dark { color: hsl( var(--clr-dark) );}
.text-accent { color: hsl( var(--clr-light) );}
.text-white { color: hsl( var(--clr-white) );}
```

Another thing I like is `grid-template-area`, makes the layout very easy to implement.

```css
.grid-container--destination {
  --flow-space: 2rem;
  grid-template-areas:
    '. title title .'
      '. image tabs .'
      '. image content .';
}
```

### Continued development

I think grid is really, really useful here when you got a complex layout of content, but I don't grasp the fundamentals that much in this project. Some of the issues I have with it are content overflow and assign an area for a piece of content.

I'm definitely learning Sass/SCSS simply because I tried and I like how efficient it is. Utility Classes like I saw in this project can go straight to partial and `@use` it in my main Sass/SCSS file.

### Useful resources

[A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - This helped me through CSS Grid. Nice and clear visuals.

## Author

- Website - [I don't have a website for now, I'm planning to create one soon!]()
- Frontend Mentor - [@nerometa](https://www.frontendmentor.io/profile/nerometa)
- GitHub - [@Ahmed5xp](https://github.com/Ahmed5xp)

