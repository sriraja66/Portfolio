# AI Coding Agent Instructions for Modern Portfolio Project

## Project Overview
This is a single-page static portfolio website built with vanilla HTML and CSS. The entire application resides in `modern_portfolio.html`, featuring a dark theme with animated elements and responsive design.

## Architecture
- **Single-file structure**: All HTML, CSS, and content in one file
- **Component organization**: Sections divided by `<section>` tags with IDs (home, about, skills, projects, contact)
- **Styling approach**: Embedded CSS with CSS custom properties for theming
- **No JavaScript**: Pure HTML/CSS implementation with CSS animations

## Key Patterns & Conventions

### CSS Theming
Use CSS custom properties defined in `:root` for consistent theming:
```css
--bg-dark: #1B1B1B;
--accent: #32FF7E;
--text-primary: #ffffff;
```
Always reference these variables instead of hardcoded colors.

### Layout Structure
Follow the established section pattern:
```html
<section id="section-name">
    <div class="container">
        <h2 class="section-title">Section Title</h2>
        <!-- Content -->
    </div>
</section>
```

### Grid Systems
Use CSS Grid for responsive layouts:
- Skills/Projects: `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr))`
- Features/Strengths: `grid-template-columns: repeat(auto-fit, minmax(250px, 1fr))`

### Animation Patterns
- Keyframe animations for entrance effects (fadeInUp, slideIn, etc.)
- Hover transforms: `transform: translateY(-10px) scale(1.05)`
- Staggered animations with `animation-delay` on nth-child selectors

### Responsive Design
- Container max-width: 1200px
- Mobile breakpoints at 768px
- Hide navigation links on mobile with `display: none`

## Development Workflow
- **Editing**: Modify `modern_portfolio.html` directly
- **Preview**: Open file in browser or use VS Code Live Server
- **No build process**: Changes are immediate
- **No dependencies**: Only Font Awesome CDN link required

## Content Updates
- Update personal information in hero and about sections
- Add new skills to `.skills-grid` following existing card structure
- Add projects to `.projects-grid` with consistent styling
- Modify contact links with actual URLs

## File References
- `modern_portfolio.html`: Complete application - examine for all patterns and styling approaches