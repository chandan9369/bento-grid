# Frontend Mentor - Bento grid solution

This is a solution to the [Bento grid challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - Bento grid solution](#frontend-mentor---bento-grid-solution)
   - [Table of contents](#table-of-contents)
   - [Overview](#overview)
      - [The challenge](#the-challenge)
      - [Screenshot](#screenshot)
      - [Links](#links)
   - [My process](#my-process)
      - [Built with](#built-with)
      - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- Experience a responsive bento grid layout that adapts from desktop to mobile seamlessly

### Screenshot

![Desktop View](./design/desktop-design.jpg)
![Mobile View](./design/mobile-design.jpg)

### Links

- Solution URL: [GitHub Repository](https://github.com/chandan9369/bento-grid)
- Live Site URL: [Live Demo](https://chandan9369.github.io/bento-grid/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid Layout
- Flexbox
- Mobile-first workflow
- DM Sans Variable Font
- Responsive design principles

### What I learned

This project was an excellent opportunity to practice advanced CSS Grid techniques. Some key learnings include:

**1. Complex Grid Areas**
Using `grid-template-areas` to create a sophisticated bento-style layout:

```css
.body-container {
   display: grid;
   grid-template-columns: repeat(4, 1fr);
   grid-template-areas:
      "box-7 box-1 box-1 box-4"
      "box-7 box-1 box-1 box-4"
      "box-8 box-2 box-3 box-4"
      "box-8 box-6 box-5 box-5";
}
```

**2. Responsive Grid Restructuring**
Learning to completely reorganize grid areas for different screen sizes:

```css
@media (max-width: 640px) {
   .body-container {
      grid-template-columns: 1fr;
      grid-template-areas:
         "box-1"
         "box-2"
         "box-3"
         "box-4"
         "box-5"
         "box-6"
         "box-7"
         "box-8";
   }
}
```

**3. Flexible Content Layouts**
Combining Grid for the overall structure with Flexbox for individual card layouts allowed for precise control over content positioning.

**4. Variable Fonts**
Implementing DM Sans variable font with different weights and styles:

```css
@font-face {
   font-family: "DM Sans";
   src: url("./assets/fonts/DMSans-VariableFont_opsz,wght.ttf")
      format("truetype");
   font-weight: 100 1000;
}
```

---

**Project Completed**: January 2026
