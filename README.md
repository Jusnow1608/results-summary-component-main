# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

#### Desktop Layout
![Desktop Layout](./solution/solution-desktop.jpg)

*The final 2-column desktop view showing the precise visual balance, responsive scaling, typography hierarchy, and organized layout.*

#### Mobile Layout
![Mobile Layout](./solution/solution-mobile.jpg)

*The responsive full-width single-column layout optimized for smaller viewports, featuring fluid padding and adjusted mobile-first spacing.*

### Links

- Solution URL: [Frontend Mentor Solution](https://www.frontendmentor.io/solutions/results-summary-component-built-with-semantic-html-css-grid-flexbox-vF6QzsjKb7)
- Live Site URL: [GitHub Pages Live Preview](https://jusnow1608.github.io/results-summary-component-main/)

## My process

### Built with

- Semantic HTML5 markup (including proper landmarks like `<main>` and structural lists)
- CSS Grid (for the primary 2-column desktop component distribution)
- Flexbox (for flexible inner alignment of scores and layout elements)
- CSS Custom Properties (Variables) for centralized color management
- Mobile-first approach & Media Queries utilizing relative units (`rem`, `em`) for accessibility
- Google Fonts integration with performance-optimized `preconnect` links

### What I learned

During this project, I significantly advanced my understanding of modern CSS structuring, web accessibility, and performance optimization. 

I practiced creating clean semantic structures by separating presentation from document flow. Wrapping core components into standalone, meaningful HTML tags ensures better compatibility with screen readers:

```html
<main class="pricing-container">
  <div class="pricing-plan">
    </div>
</main>
```
On the CSS side, I mastered the usage of CSS variables to keep the code DRY (Don't Repeat Yourself) and applied consistent styling across global components:

```CSS
:root {
  --color-primary: hsl(245, 75%, 52%);
  --color-bg-page: hsl(225, 100%, 94%);
  --color-container-box-shadow: rgba(56, 41, 224, 0.04);
}

body {
  background-color: var(--color-bg-page);
}
```
I also learned how to handle background scaling effectively without stretching or distorting decorative patterns across ultra-wide viewports, utilizing CSS functions and properties correctly to preserve the user experience:

```CSS
body {
  background-image: url("images/pattern-background-desktop.svg");
  background-repeat: no-repeat;
  background-size: contain;
  background-position: top center;
}
```
### Continued development
In future projects, I want to focus more on:

- Deepening knowledge of BEM (Block Element Modifier) methodology for predictable CSS architecture.

- Advanced responsive layouts utilizing dynamic CSS functions like clamp(), min(), and max().

- Expanding my knowledge on WCAG guidelines to deliver fully accessible digital products.

### AI Collaboration
I collaborated with Gemini AI as an interactive peer code-reviewer during this project.

- How I used it: I used the AI assistant to auditing my CSS code architecture, cleaning up unused components, and pinpointing layout bugs.

- What worked well: The collaborative refactoring process was excellent for catching critical syntax and logic slips. The assistant guided me to identify a missing semicolon in my custom properties, an unintended dot prefixing a body tag within media queries, and optimized an interactive button state where an abrupt hover border was triggering layout shift ("jumping text").

## Author

- GitHub - [@Jusnow1608](https://github.com/Jusnow1608)
- Frontend Mentor - [@Jusnow1608](https://www.frontendmentor.io/profile/Jusnow1608)
- LinkedIn - [@Justyna-Nowak-Szrajnert](https://www.linkedin.com/in/justyna-nowak-szrajnert-a5168713b/)

