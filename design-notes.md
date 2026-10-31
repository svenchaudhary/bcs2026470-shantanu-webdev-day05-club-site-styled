
# Design notes — Day 5

## Design direction

- Site purpose and audience: Campus Connect is a college club website for students of Invertis University.
- Visual style / mood: Modern, clean, professional, welcoming, and student-friendly.
- Student: Shantanu Chaudhary
- Course: B.Tech Computer Science Engineering
- Batch: 2026

## Colour palette

| Role | Colour value | Where it is used |
|---|---|---|
| Primary | #2458a6 | Header, buttons, links |
| Secondary | #17243a | Footer and main text |
| Accent | #e5a93d | Highlights and accents |
| Page background | #f3f6fb | Main page background |
| Main text | #17243a | Headings and body text |
| Surface | #ffffff | Cards and forms |

## Typography

- Google Font for headings: Manrope
- Google Font for body text: DM Sans
- Why these fonts work for the site: Manrope gives headings a modern and bold appearance, while DM Sans makes paragraphs and form labels easy to read.

## CSS design tokens

| Custom property | Value | Purpose |
|---|---|---|
| --color-primary | #2458a6 | Main brand colour |
| --color-accent | #e5a93d | Highlights |
| --space-1 | 0.5rem | Small spacing |
| --space-2 | 1rem | Normal spacing |
| --space-3 | 1.5rem | Section spacing |
| --font-body | DM Sans | Body typography |
| --font-heading | Manrope | Heading typography |

## Selectors and cascade

The stylesheet uses:
- Element selector: body, h1, p, table
- Class selector: .hero, .card, .form-card
- ID selector: #join-us
- Descendant selector: .site-header nav a
- Attribute selector: input[type="submit"]
- Pseudo-class selector: a:hover

Class-versus-ID test:
I applied the .section class and #join-us ID to the same section. I inspected the declarations in browser DevTools. The ID selector has higher specificity than the class selector, so its background-color declaration wins when both selectors set that property.

## DevTools debugging

- Issue found: I checked whether the stylesheet was loading on all pages and whether form fields fit on narrow screens.
- How I found it: I used browser DevTools, the Elements panel, and responsive device mode.
- Fix: I corrected stylesheet paths, used responsive grid layouts, added max-width rules, and checked form field widths.

## Final review

- Pages checked: index.html, about.html, registration.html, contact.html
- Screenshot filename: campus-connect-day5.png
- Repository URL: Add your GitHub repository URL here.
