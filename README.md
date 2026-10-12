# Shaniel-MPOFU

A semantic HTML5 mini-portfolio for a Computer Information Systems student at Africa University. This version applies the Unit III responsive styling requirements while preserving the existing profile content and accessible contact form.

## About the Project

The page contains:
- An About Me section
- Skills and personal interests
- A Contact Me form
- A footer

The contact form keeps the name, email address, and phone number pre-filled and read-only. Visitors can enter a message. The form is a front-end demonstration and does not send data to a server.

## Technologies Used

- HTML5 semantic elements
- CSS3
- Flexbox
- CSS Grid
- Mobile-first media queries
- Tailwind CSS utility classes
- Git and GitHub

Tailwind's Play CDN is used for this coursework prototype. It is convenient for development and demonstration, but a compiled Tailwind build is recommended for production deployment.

## Project Structure

```text
Shaniel-MPOFU/
├── index.html
├── style.css
├── README.md
└── PROMPT_LOG.md
```

## Responsive Notes

### Breakpoints tested

Target viewport widths for browser testing:
- Mobile: 375px
- Tablet: 768px
- Desktop: 1280px

Before submission, open the page in browser Developer Tools and check all three widths. Confirm that there is no horizontal overflow, navigation remains usable, text wraps correctly, the skills cards fit their containers, and form controls remain within the page. Record only tests that you have actually completed.

### Mobile-first approach

The base CSS is designed for narrow screens first. `min-width` media queries at 600px and 900px add spacing and adapt the layout for larger viewports. The CSS also respects the user's reduced-motion preference.

### Flexbox vs. Grid

- **Flexbox:** The navigation uses Tailwind Flexbox utilities to centre and space links. It changes from a vertical layout to a horizontal, wrapping layout at Tailwind's `sm` breakpoint. The contact-form fields use custom Flexbox to stack labels and controls consistently.
- **CSS Grid:** The skills section uses `grid-template-columns: minmax(0, 1fr)` on mobile and `repeat(2, minmax(0, 1fr))` from 600px upward. This makes the cards reflow into two equal columns on wider screens.

### Tailwind utility classes

- **Header:** Tailwind utilities set responsive padding, text alignment, heading size, and spacing.
- **Navigation:** Tailwind utilities control Flexbox layout, alignment, gaps, and the responsive direction.
- **Contact form:** Tailwind utilities establish a one-column grid and consistent gaps.

Custom CSS controls the colour palette, typography, box model, card styling, inputs, focus indicators, skills grid, and custom media queries. This split is intentional to avoid styling the same layout properties in both systems.

## Accessibility

- Semantic `header`, `nav`, `main`, `section`, `article`, and `footer` elements are used.
- The navigation has an accessible label.
- Form labels are associated with their inputs.
- The message field is required and has a minimum length.
- Keyboard focus indicators are visible.
- The page uses responsive sizing and avoids fixed-width content cards.

## Version Control

Use a series of focused commits rather than one final commit. Suggested commit messages:

1. `Refine CSS box model and typography`
2. `Add responsive Flexbox navigation`
3. `Implement responsive CSS Grid for skills`
4. `Add mobile-first media queries`
5. `Apply Tailwind utilities to header and contact form`
6. `Document responsive design and testing`

These are suggested messages for the changes you make. Do not claim browser testing or create a commit until the corresponding work has actually been completed.

## Author

**Shaniel Mpofu**  
Computer Information Systems  
Africa University
