# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor]

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

This is a challenge featuring a header and four cards arranged in a grid layout with different views for desktop and mobile.

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![DESKTOP VIEW](/assets/desktop-screenshot.png)
![MOBILE-VIEW](/assets/mobile-screenshot.png)

## My process

I started with laying out the html structure. I have used semantic tags neatly dividing the page into a header and four sections then wrapping the four sections into a div container setting the display to grid. Following this i used css styles to style the page, firstly styling for mobile view and then the desktop view.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I could have wrapped the second column cards in the desktop view in a div and used flex or maybe inline grid to arrange them but i wanted to stick to the grid view set in the parent container as this would have made styling the four cards much easier and also wouldn't have affected the mobile view and the size of the cards so arranging the grid items according to the row and column number is something very new that i learnt. Then i used translate functions on column 1 and 3 cards to move them to the middle.
This is the part i learnt.
.container {
display: grid;
grid-template-columns: repeat(3, 1fr);
grid-template-rows: repeat(2, 1fr);
row-gap: 20px;
column-gap: 20px;
max-width: 1000px;
}
.supervisor {
grid-column: 1;
grid-row: 1;
transform: translateY(50%);
}
.team-builder {
grid-column: 2;
grid-row: 1;
}

.calculator {
grid-column: 3;
grid-row: 1;
transform: translateY(50%);
}

.karma {
grid-column: 2;
grid-row: 2;
}
