# Testimonials Grid Section

A responsive testimonials grid showcasing student testimonials in an elegant multi-column layout. Built as part of the [Frontend Mentor](https://www.frontendmentor.io/) Building Responsive Layouts learning path.

## 🎯 Overview

This project demonstrates a testimonials grid section featuring five student testimonials. The layout adapts seamlessly from a single-column mobile view to a sophisticated multi-column grid on desktop screens.

### Solution

![Testimonials Grid Section](./images/solution.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/hakan-kemal/testimonials-grid-section)
- Live Site URL: [Netlify Deployment](https://testimonials-grid-section-hk.netlify.app/)

## 🛠 My Process

### Built With

- **HTML5** - Semantic markup
- **CSS3** - Modern styling techniques
  - CSS Custom Properties (CSS Variables)
  - CSS Grid Layout
  - Flexbox Layout
  - Mobile-first workflow
- **Google Fonts** - [Barlow Semi Condensed](https://fonts.google.com/specimen/Barlow+Semi+Condensed)

### What I Learned

This project reinforced several key concepts:

**CSS Grid Layouts:** Created a responsive testimonial grid using CSS Grid with named template areas:

```css
.testimonials-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-areas:
    'daniel daniel jonathan kira'
    'jeanette patrick patrick kira';
}

.testimonial-daniel {
  grid-area: daniel;
}
```

**CSS Custom Properties:** Organized color, typography, and spacing values using CSS variables for maintainability:

```css
:root {
  /* Colors */
  --color-purple-500: hsl(263, 55%, 52%);
  --color-grey-500: hsl(217, 19%, 35%);
  --color-dark-blue: hsl(219, 29%, 14%);
  --color-white: hsl(0, 0%, 100%);
  /* Spacing */
  --spacing-200: 1rem;
  --spacing-400: 2rem;
  /* Typography */
  --font-weight-base: 500;
  --font-weight-semi-bold: 600;
}
```

**Responsive Design:** Implemented mobile-first approach with seamless breakpoints:

```css
@media (min-width: 48rem) {
  .testimonials-container {
    grid-template-columns: repeat(2, 1fr);
    grid-template-areas:
      'daniel daniel'
      'jonathan jeanette'
      'patrick patrick'
      'kira kira';
  }
}

@media (min-width: 90rem) {
  .testimonials-container {
    grid-template-columns: repeat(4, 1fr);
    grid-template-areas:
      'daniel daniel jonathan kira'
      'jeanette patrick patrick kira';
  }
}
```

### Continued Development

Areas I want to focus on in future projects:

- Exploring more complex CSS Grid patterns and asymmetric layouts
- Learning CSS subgrid for nested grid layouts
- Adding JavaScript interactivity to components
- Implementing CSS animations and transitions for better UX
- Improving accessibility with proper ARIA attributes and keyboard navigation

### Useful Resources

- [MDN Web Docs - CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout) - Comprehensive guide on CSS Grid
- [CSS-Tricks - A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) - Excellent visual reference for Grid properties
- [web.dev - CSS Custom Properties](https://web.dev/learn/css/custom-properties) - Understanding CSS variables

## 👤 Author

- Frontend Mentor - [@hakan-kemal](https://www.frontendmentor.io/profile/hakan-kemal)
- GitHub - [@hakan-kemal](https://github.com/hakan-kemal)

## 🙏 Acknowledgments

Thanks to Frontend Mentor for providing this challenge and the design specifications.
