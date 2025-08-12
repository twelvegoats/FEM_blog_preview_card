# Frontend Mentor - Blog Preview Card Solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Useful Resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the blog preview card
- See a responsive design that works on both mobile and desktop devices
- Experience a clean, accessible card component with proper semantic structure

### Screenshot

![](./preview.jpg)

### Links

- Solution URL: [GitHub Repository](https://github.com/twelvegoats/FEM_blog_preview_card)
- Live Site URL: [Live Demo](https://twelvegoats.github.io/FEM_blog_preview_card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (CSS Variables)
- Flexbox
- BEM (Block Element Modifier) methodology
- Custom font implementation

### What I learned

This project was an excellent opportunity to practice and solidify several key frontend development concepts:

#### 1. BEM (Block Element Modifier) Methodology

One of the main focuses of this project was implementing the BEM naming convention for CSS classes. This methodology helped me create more maintainable and scalable CSS:

```html
<div class="blog-card">
  <div class="blog-card__image-container">
    <img class="blog-card__image" />
  </div>
  <div class="blog-card__content">
    <span class="blog-card__category">Learning</span>
    <time class="blog-card__date">Published 21 Dec 2023</time>
    <h1 class="blog-card__title">HTML & CSS foundations</h1>
    <p class="blog-card__description">...</p>
    <div class="blog-card__author">
      <img class="blog-card__author-avatar" />
      <span class="blog-card__author-name">Greg Hooper</span>
    </div>
  </div>
</div>
```

Benefits I discovered with BEM:

- **Clear component structure:** Each class name clearly indicates its relationship to the parent block
- **Reduced CSS specificity conflicts:** No need for deeply nested selectors
- **Better maintainability:** Easy to understand which styles belong to which component
- **Reusability:** Components can be easily moved or reused without breaking styles

#### 2. CSS Custom Properties (Variables)

I implemented a comprehensive design system using CSS custom properties:

```
:root {
  /* Color Palette */
  --yellow: #f4d04e;
  --gray-950: #111111;
  --gray-500: #6b6b6b;
  --white: #ffffff;

  /* Typography */
  --text-preset-1-font-weight: 900;
  --text-preset-1-font-size: 1.5rem;
  --text-preset-2-font-weight: 400;
  --text-preset-2-font-size: 1rem;
  --text-preset-3-font-size: 0.875rem;
  --line-height: 150%;

  /* Spacing */
  --spacing-300: 1.5rem;
  --spacing-150: 0.75rem;
  --spacing-100: 0.5rem;
  --spacing-50: 0.25rem;
}
```

This approach taught me:

- How to create a consistent design system
- The importance of maintaining design tokens
- How CSS variables improve maintainability and theme consistency

#### 3. Modern CSS Layout Techniques

I utilized Flexbox for component layout and centering:

```
main {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.blog-card__author {
  display: flex;
  align-items: center;
}
```

#### 4. Semantic HTML Structure

I focused on using semantic HTML elements for better accessibility and SEO:

```
<main>
  <article class="blog-card">
    <time class="blog-card__date">Published 21 Dec 2023</time>
    <h1 class="blog-card__title">HTML & CSS foundations</h1>
  </article>
</main>
```

#### 5. Custom Font Implementation

I learned how to properly implement custom fonts using @font-face:

```
@font-face {
  font-family: 'Figtree';
  src: url('../assets/fonts/Figtree-VariableFont_wght.ttf');
}
```

#### 6. Box Shadow and Visual Effects

implemented the design's distinctive shadow effect:

```
.blog-card {
 box-shadow: 8px 8px var(--gray-950);
}
```

### Key Takeaways

- **BEM methodology** significantly improved my CSS organization and made the codebase more maintainable
- **CSS custom properties** are powerful for creating consistent design systems
- **Semantic HTML** is crucial for accessibility and proper document structure
- **Flexbox** provides elegant solutions for layout challenges
- **Design tokens** (spacing, typography, colors) help maintain consistency across a project

### Continued development

In future projects, I want to continue focusing on:

- Advanced BEM patterns and modifiers
- CSS Grid for more complex layouts
- Accessibility improvements (ARIA labels, keyboard navigation)
- Performance optimization techniques
- Responsive design patterns

## Useful Resources

- [BEM Methodology](https://getbem.com/) - Comprehensive guide to BEM naming conventions
- [CSS Custom Properties Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_cascading_variables/Using_CSS_custom_properties) - MDN documentation on CSS variables
- [Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Complete guide to Flexbox by [CSS-TRICKS](https://css-tricks.com/)

### Author

- website - [Sean Wildman](https://github.com/twelvegoats)
- Frontend Mentor - [@twelvegoats](https://www.frontendmentor.io/profile/twelvegoats)
