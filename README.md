# LUMIÈRE — Fine Dining & Culinary Art

A single-page restaurant website for **LUMIÈRE**, a fictional upscale fine-dining restaurant. Built as one self-contained HTML file with embedded CSS and JavaScript — no build step required.

## Preview

Open `index.html` directly in any modern browser (requires an internet connection for fonts, icons, and the animation library loaded via CDN).

## Sections

| Section | Content |
|---|---|
| **Nav** | Fixed, blurred navigation bar with logo and a "Book Table" CTA |
| **Hero** | Full-height intro with gradient headline text and a floating, slowly rotating dish photo inside a dashed ring |
| **About** | Restaurant story, two-image grid, and a note on the executive chef |
| **Menu** | Tabbed menu browser (Main Courses / Starters / Desserts & Drinks) with photo cards, item names, descriptions, and prices |
| **Reservation** | Booking form (name, email, date, time slot, guest count, special requests) |
| **Contact & Location** | Address, phone, hours, and an embedded Google Map (styled grayscale) |
| **Footer** | Logo, social icons, and copyright |

## Tech

- **Fonts:** Cinzel (display serif headings), Plus Jakarta Sans (body) — loaded from Google Fonts
- **Icons:** Font Awesome 6 (via CDN)
- **Animation:** [AOS (Animate On Scroll)](https://michalsnik.github.io/aos/) for scroll-reveal effects on section entry
- **No frameworks** — vanilla HTML/CSS/JS in a single file
- **CSS custom properties** for the dark/gold color palette and typography, defined in `:root`
- Responsive breakpoint at 968px (stacks hero, about, contact, and reservation form into single columns; hides nav links)

## Interactive behaviors

- **Ambient glow** — a soft gold radial gradient that drifts diagonally across the page in a continuous loop
- **Hero image** — rotates and gently bobs on a 25s loop, with a separate dashed ring counter-rotating around it
- **Menu tabs** — clicking a category swaps the visible menu-card grid via `switchTab()`
- **Reservation form** — client-side only; submitting shows a JS `alert()` confirmation, no backend or data storage

## Notes

- Menu photography and hero/about images are hotlinked from Unsplash
- The embedded map and address are placeholder/sample data, not a real location
- Footer social links are placeholders (`href="#"`)
- No mobile hamburger menu — nav links are simply hidden below 968px width
