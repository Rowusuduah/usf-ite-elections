# USF ITE Elections — CLAUDE.md

## Project Overview

Static single-page site for the USF Institute of Transportation Engineers 2026–2027 Executive Board Elections. Displays candidate statements and links to BullsConnect for voting. Hosted on GitHub Pages.

## File Structure

```
USF ITE ELECTIONS/
├── index.html        # Single-file static page (HTML + embedded CSS, no JS)
└── .gitignore
```

## Architecture

- Pure static HTML — no JavaScript, no build tools, no frameworks
- All CSS is embedded in a `<style>` block inside `index.html`
- Google Fonts loaded externally (DM Serif Display, DM Sans)
- USF brand colors: green (#00843D), gold (#CFC493), dark (#0D1F14)
- Responsive breakpoints at 700px and 480px

## External Links

- **BullsConnect (voting)**: https://bullsconnect.usf.edu
- **Google Drive video**: Jeremy Fullwood's intro video
- **LinkedIn**: Le Nguyen's profile
- **Email**: lehuuthucnguyen@usf.edu

## Coding Conventions

- All candidate statements are displayed exactly as submitted (preserve whitespace via `white-space: pre-wrap`)
- Candidate avatars show initials via CSS (no images)
- Use CSS custom properties (design tokens) defined in `:root`
- Do not add JavaScript unless explicitly requested
- Keep everything in a single `index.html` file

## Deployment

- GitHub Pages from `main` branch root
- No build step required — files served as-is
