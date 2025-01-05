# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)



## Overview

<a href="https://junmike-blog-preview.netlify.app/" target="_blank">View Live Website</a>
</br>
<img src="https://raw.githubusercontent.com/MichaelDAbadJr/assets/refs/heads/main/blog-preview-cover.png" width="600">

link to the repository -->
<a href="https://github.com/MichaelDAbadJr/Blog-Preview-Card" target="_blank">Blog-Preview Repository</a>

## My process
I used the figma design to extract measurements such as the font, text size, text weight, padding, margin, and gaps, etc. I Focused on scalability and making presets for fonts and defining :root css variables.

### Built with
CSS Reset:
Including margin: 0; padding: 0; box-sizing: border-box; ensures a consistent design across browsers.

Root Variables:
Using :root for color variables, font weight variables, and fonts, excellent for scalability and maintainability. It makes it easier to update the text theme and reuse colors.

Typography:
The Google Font Montserrat and Fraunces is applied consistently, and the font weights (400 and 700) are preloaded for performance optimization.

Responsive Design:
Using max-width for the .product container ensures the design remains responsive across devices.
The use of min-height: 100svh for the body ensures the card is always vertically centered in the viewport.

Semantic HTML:
Using main for the card container is semantically correct because it represents the main content of the page.

Gridbox:
Gridbox is used effectively for centering and aligning content, both for the overall layout and within the card. The body is set to a grid container, which ensures that all of its children (in this case, the main content of the page) are centered both vertically and horizontally.
min-height: 100svh: This ensures the grid container covers at least 100% of the viewport height (with svh being a more consistent unit across devices).
place-content: center: This property centers the content both horizontally and vertically in the grid container.
margin: 1rem: This adds spacing around the body, which ensures the content doesn’t touch the edges of the viewport.
Grid on .product: The .product container is also set to a grid layout, which allows for a flexible internal structure. The grid is used here to manage the layout of the product's image and content (description, price, etc.).
Max-width: The max-width: 600px ensures that the product card doesn't grow too wide and remains a manageable size on larger screens.
Grid columns for larger screens: When the viewport width is at least 768px (usually tablets and larger screens), the .product grid is split into two columns (1fr 1fr). One column will contain the image, and the other will contain the content.
grid-template-columns: 1fr 1fr: This creates two equal-width columns, where 1fr means "1 fraction of the available space."
Grid on .product__content: The .product__content section is a grid container for the textual content (category, title, price, and button). Using grid here allows you to easily manage the spacing between elements.
gap: var(--content-spacing): This sets the spacing between grid items.
padding: var(--content-padding): This adds padding inside the content area to ensure that the text doesn’t touch the edges of its container.

### What I learned
The grid layout is used to structure elements in the body, product card, and product content sections.
The body grid centers the content vertically and horizontally.
The .product grid controls the layout of the product card, including its image and content.
The .product__content uses grid to space out the individual elements of the product description.
On larger screens, media queries switch the product layout to a two-column grid, making the design responsive.
In general, grid is used here to create a flexible and responsive layout that adjusts based on the screen size while maintaining proper spacing and alignment.


## Author
- Website - [JunMike](https://junmike.dev)
- Frontend Mentor - [@MichaelDAbadJr](https://www.frontendmentor.io/profile/MichaelDAbadJr)