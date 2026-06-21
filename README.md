# ATHASH Digital Solutions — Website v4

> **File:** `athash-website-v4.html`
> **Type:** Single-file HTML website (no build tools, no dependencies, no server required)
> **Last Updated:** June 2026

---

## What This Is

A complete, production-ready marketing website for **ATHASH Digital Solutions** — a South African business providing company registration, branding, web design, and IT support services.

The entire website lives in **one HTML file**. Open it in any browser and it works. Upload it to any web host and it's live.

---

## File Structure

```
athash-website-v4.html   ← Everything. HTML + CSS + JS + images (base64 embedded)
README.md                ← This file
```

All images (logo and founder photo) are embedded as base64 data URIs inside the HTML, so the file is fully self-contained — no missing image links.

---

## Sections (Top to Bottom)

| # | Section | Purpose |
|---|---------|---------|
| 1 | **Navigation** | Fixed top bar with logo, links, CTA button, hamburger on mobile |
| 2 | **Hero** | Headline, subline, body copy, two CTA buttons, Launch→Grow→Succeed journey indicator |
| 3 | **Stats Strip** | Animated counters: Businesses Supported, Websites Built, Projects Completed |
| 4 | **Carousel** | Auto-advancing 6-slide highlight reel with progress bar, dots, swipe support |
| 5 | **Quick Contact Widget** | "What Do You Need?" — 5 category buttons that reveal a tailored WhatsApp form |
| 6 | **Outcomes** | Three outcome cards: Launch / Grow / Support — for different client stages |
| 7 | **Startup Package** | Feature list + pricing card for the flagship R4,999 bundle |
| 8 | **Package Builder** | Interactive checklist — visitor selects services, live price estimate updates |
| 9 | **Other Packages** | Digital Growth Package + IT Support Package |
| 10 | **Pricing Guide** | 4-tile pricing reference grid |
| 11 | **Portfolio** | 3 before/after transformation stories with outcomes |
| 12 | **Testimonials** | 3 client review cards with star ratings |
| 13 | **About** | Founder photo, bio, contact details, brand story |
| 14 | **CTA Strip** | Phone number + Call / WhatsApp buttons |
| 15 | **Contact** | Contact cards + full enquiry form |
| 16 | **Footer** | Brand, pillars, copyright |
| — | **WhatsApp Float** | Fixed bottom-right WhatsApp bubble (always visible) |

---

## Features

### Navigation
- Fixed header with blur/glass effect
- Logo image (left), nav links (centre), CTA button (right)
- **Hamburger menu on mobile** — slides in a right drawer with overlay
- Links shrink the nav height on scroll
- Active link closes the mobile drawer automatically

### Carousel
- 6 slides: stats, selling points, pricing anchor
- **Auto-advances every 4 seconds** with a gold progress bar
- Arrow buttons (left/right)
- Dot navigation — jumps to any page
- **Touch & swipe support** for mobile
- Pauses on hover (desktop)
- Responsive: 3 slides/view → 2 on tablet → 1 on mobile

### Interactive Package Builder
- Tick any combination of 6 services
- Live price estimate updates instantly
- "Request This Package" CTA appears once selections are made

### Quick Contact Widget
- 5 service category buttons
- Reveals a short form tailored to the selected service
- **Submits directly to WhatsApp** with name, phone, and service pre-filled in the message

### Scroll Animations
- Every section fades and rises in as it enters the viewport
- Counter numbers animate from 0 to their target value on scroll

---

## Colours

| Token | Hex | Usage |
|-------|-----|-------|
| `--navy` | `#0B1628` | Page background |
| `--navy-mid` | `#112240` | Card / section backgrounds |
| `--navy-lit` | `#1a3260` | Hover states, gradients |
| `--gold` | `#C9921A` | Primary brand accent |
| `--gold-lt` | `#E8B84B` | Headings, highlights |
| `--gold-pale` | `#f5d98b` | Subtle gold tints |
| `--muted` | `#8CA0C0` | Body text, labels |
| `--white` | `#FFFFFF` | Primary text |
| `--off-white` | `#F0F4FF` | List items, secondary text |

---

## Fonts

Loaded from Google Fonts (requires internet connection):

- **Montserrat** (400–900) — Headings, logo, buttons, labels
- **Inter** (300–600) — Body text, form fields

> **Offline fallback:** If Google Fonts is unavailable, the browser falls back to system sans-serif fonts.

---

## Contact Details (Currently in the site)

| Field | Value |
|-------|-------|
| Phone / WhatsApp | 082 056 9497 |
| Email | hello@athash.co.za |
| Website | www.athash.co.za |
| WhatsApp link | https://wa.me/27820569497 |

To update any of these, search the HTML file for the value and replace all instances.

---

## How to Deploy

### Option 1 — Direct upload (simplest)
Upload `athash-website-v4.html` to any web host as `index.html`.

### Option 2 — GitHub Pages (free)
1. Create a GitHub repository
2. Upload the file as `index.html`
3. Go to **Settings → Pages → Deploy from main branch**
4. Your site is live at `https://yourusername.github.io/repo-name`

### Option 3 — Netlify (free, custom domain)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop the HTML file onto the Netlify dashboard
3. Site is live in seconds — connect your domain in settings

### Option 4 — cPanel / shared hosting
1. Log into your hosting control panel
2. Open **File Manager → public_html**
3. Upload the file and rename it `index.html`

---

## How to Edit

Since this is a single HTML file, everything is in one place:

| What to change | Where to find it |
|----------------|-----------------|
| Business name, phone, email | Search the file for the current value |
| Pricing | Search for `R4,999`, `R2,999`, etc. |
| Testimonials | Find `<!-- TESTIMONIALS -->` section |
| Portfolio stories | Find `<!-- PORTFOLIO -->` section |
| Logo image | Replace the `data:image/png;base64,...` inside the nav `<img>` tag |
| Founder photo | Replace the `data:image/png;base64,...` inside the `.founder-avatar` `<img>` tag |
| Carousel slides | Find `<!-- CAROUSEL -->` and edit `.carousel-slide` blocks |
| WhatsApp number | Search for `wa.me/27820569497` — replace the number part |
| Colour scheme | Edit CSS variables in `:root { }` at the top of the `<style>` block |

---

## Browser Support

| Browser | Support |
|---------|---------|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari (iOS & Mac) | ✅ Full |
| Samsung Internet | ✅ Full |
| Opera | ✅ Full |
| IE 11 | ❌ Not supported (CSS variables not supported) |

---

## Responsive Breakpoints

| Breakpoint | Layout |
|------------|--------|
| `> 1200px` | Full desktop — 3-column grids, carousel shows 3 slides |
| `961px – 1200px` | Medium desktop — 2-column grids, carousel shows 2 slides |
| `≤ 960px` | Mobile — single column, hamburger nav, carousel shows 1 slide |

---

## Version History

| Version | File | Changes |
|---------|------|---------|
| v1 | `athash-website.html` | Original uploaded file |
| v2 | `athash-website-v2.html` | Full redesign based on strategy critique |
| v3 | `athash-website-v3.html` | Real logo + founder photo embedded |
| v4 | `athash-website-v4.html` | Clean nav, hamburger menu, carousel, hero gap fix |

---

## Credits

**Design & Development:** Built for ATHASH Digital Solutions  
**Founder:** Snethemba Ngcobo  
**Logo & Photo:** ATHASH brand assets  

---

*© 2025 ATHASH Digital Solutions. All rights reserved.*
