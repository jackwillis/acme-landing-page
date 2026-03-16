# Acme Corp Landing Page

## Project

Marketing landing page for Acme Corp — a fictional B2B SaaS company. Single-page site, no backend.

## Tech Stack

- **Single file:** Everything goes in `index.html`
- **Tailwind CSS:** Load via CDN (`<script src="https://cdn.tailwindcss.com"></script>`)
- **Vanilla JS only** — no frameworks, no build step
- **Must work by opening the HTML file directly in a browser** (no server required)

Inline styles and scripts are fine, but prefer Tailwind utility classes over custom CSS.

## Brand Guidelines

### Colors

| Role | Value | Tailwind |
|------|-------|----------|
| Primary | #2563EB | `blue-600` |
| Secondary | #1E40AF | `blue-800` |
| Accent | #F59E0B | `amber-500` |
| Background | #FFFFFF | `white` |
| Text | #1F2937 | `gray-800` |

### Typography

Use [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts. Load in `<head>`:

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

Set as the default font via Tailwind config:

```html
<script>
  tailwind.config = {
    theme: {
      fontFamily: {
        sans: ['Inter', 'system-ui', 'sans-serif'],
      }
    }
  }
</script>
```

### Logo

Use the SVG at `assets/acme-logo.svg`. Load it inline or via `<img>` tag.

## Design Constraints

- **Responsive:** Mobile-first. Must look good on phone, tablet, and desktop.
- **Tone:** Professional but friendly. Think "competent startup," not "enterprise sales deck."
- **Accessibility:** Semantic HTML, sufficient color contrast, alt text on images.
- **No placeholder images:** Use SVG illustrations, CSS gradients, or emoji as visual elements instead of broken image links.

## What NOT to Do

- Don't create additional files — everything in `index.html`
- Don't add npm, package.json, or any build tooling
- Don't use React, Vue, or any framework
- Don't hardcode viewport widths — use Tailwind responsive prefixes (`sm:`, `md:`, `lg:`)
