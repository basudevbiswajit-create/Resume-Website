# Basudev Biswajit Nath - Personal Resume Website

A responsive personal portfolio website built with plain HTML5 and CSS3 (no JavaScript) for an academic web development project (BBA in Digital Business and Entrepreneurship, IIM Bangalore).

**Live website:** https://basudevbiswajit-create.github.io/Resume-Website/

## How to open it

1. Keep index.html, style.css and basudev-portrait.jpeg in the same folder.
2. Double-click index.html. It opens in any modern browser.

No build step is needed. Headings and body text use Google Fonts (Playfair Display and DM Sans), loaded by a link tag in index.html. If you are offline, the site falls back to Georgia and your system fonts and still works.

## Files

| File | Purpose |
| --- | --- |
| index.html | Page structure and content |
| style.css | All styling (external stylesheet) |
| basudev-portrait.jpeg | Cropped portrait used in the hero section |
| README.md | This file |

## Design idea

A calm, professional look for a business and investing profile.

- **Palette:** navy, ivory and a muted gold accent, defined once as CSS variables.
- **Typography:** Playfair Display (serif) for headings, DM Sans (sans-serif) for body text and small labels.
- **Portrait:** cropped to a 4:5 ratio with an offset gold frame drawn using a CSS pseudo-element.
- **Motion:** a fade-up entrance effect done with CSS only, switched off for visitors who prefer reduced motion.

## Page structure

- Header with logo, navigation (About, Education, Experience, Skills, Contact) and a Get in touch link
- Hero: name, short introduction, two buttons and portrait with caption
- 01 About: statement and two short paragraphs
- 02 Education: timeline of IIM Bangalore, Dhenkanal Autonomous College, DPS and St. Xavier's High School
- 03 Experience: two cards (family business; forex and Indian markets)
- 04 Skills and interests: two-column lists
- 05 Contact: navy call-to-action section with email and LinkedIn links
- Footer with logo and email link

## Where each concept is used

### HTML

- **Document structure:** doctype, html, head and body elements
- **Semantic elements:** header, nav, main, section, article, figure, figcaption and footer
- **Headings and paragraphs:** h1 to h3 and p
- **Unordered lists:** skills and areas of interest
- **Anchor tags:** in-page navigation (href="#experience"), mailto links and an external LinkedIn link
- **Image:** with descriptive alt text
- **Classes and IDs:** for example class="experience-card" and id="experience"

### CSS

- **Element and class selectors:** body, a, .experience-card
- **Grouped selectors:** .nav-link, .header-contact
- **Pseudo-classes and pseudo-elements:** :hover, :focus-visible, ::before, ::selection
- **Typography, colours and fonts:** CSS variables on :root, serif headings, sans-serif body, clamp() for responsive sizes
- **Box model:** padding, margin, border, plus box-sizing: border-box
- **Cascade:** .button-light overrides the base .button styles
- **Display:** display: grid, display: flex, display: inline-flex
- **Positioning:** position: relative on the hero, position: absolute for the scroll note and portrait frame
- **Flexbox:** header, navigation, hero, buttons, footer
- **CSS Grid:** About section, education timeline, experience cards, skills lists
- **Transitions and animation:** transition on links and cards, @keyframes fade-up
- **Responsive design:** media query at 700px and a prefers-reduced-motion query

## Customising

- **Colours:** edit the variables at the top of style.css.
- **Content:** edit the text in index.html. Each section has its own id.
