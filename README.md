# ATHASH Digital Solutions — Website

> **File:** `athash-website-final.html`
> **Type:** Single-file HTML website (no build tools, no dependencies, no server required)
> **Formspree Endpoint:** `https://formspree.io/f/mykqgdko`
> **Last Updated:** June 2026

---

## What This Is

A complete, production-ready marketing website for **ATHASH Digital Solutions** — a South African business providing company registration, branding, web design, and IT support services.

The entire website lives in **one HTML file**. Open it in any browser and it works. Upload it to any web host and it's live.

All images (logo and founder photo) are embedded as base64 data URIs — no missing image links, no external assets required.

---

## File Structure

```
athash-website-final.html   ← Everything: HTML + CSS + JS + images (base64 embedded)
README.md                   ← This file
```

---

## Sections (Top to Bottom)

| # | Section | Purpose |
|---|---------|---------|
| 1 | **Navigation** | Fixed top bar — logo, dropdown nav, CTA button, hamburger on mobile |
| 2 | **Hero** | Emotional hook, headline, subline, two CTA buttons, Launch→Grow→Succeed journey |
| 3 | **Stats Strip** | Animated counters: 50+ Businesses, 30+ Websites, 80+ Projects |
| 4 | **Quick Contact Widget** | "What Do You Need?" — 5 category buttons → tailored WhatsApp form |
| 5 | **Outcomes** | Three outcome cards: Launch / Grow / Support — for different client stages |
| 6 | **Carousel** | Auto-advancing 6-slide highlight reel with progress bar, dots, swipe |
| 7 | **Startup Package** | Feature list + pricing card for the flagship R4,999 bundle |
| 8 | **Package Builder** | Interactive checklist — select services, live price estimate updates |
| 9 | **Other Packages** | Digital Growth Package + IT Support Package |
| 10 | **Pricing Guide** | 4-tile transparent pricing reference grid |
| 11 | **Portfolio** | 3 before/after transformation stories with outcomes |
| 12 | **Testimonials** | 3 client review cards with star ratings |
| 13 | **About** | Founder photo, bio, contact details, brand story |
| 14 | **CTA Strip** | Phone number + Call / WhatsApp buttons |
| 15 | **Contact** | Contact cards + Formspree-powered enquiry form |
| 16 | **Footer** | Brand, pillars, phone, WhatsApp, email, copyright |
| — | **WhatsApp Float** | Fixed bottom-right official WhatsApp SVG button (always visible) |

---

## Features

### Navigation
- Fixed header with blur/glass effect
- Logo (left) · Packages dropdown + links (centre) · CTA button (right)
- **Packages dropdown** combines: Startup Package, Build a Package, Other Packages, Pricing Guide
- **Hamburger menu on mobile** — slides in a right-side drawer with dark overlay
- Nav height reduces on scroll
- All mobile drawer links close the menu on tap

### Hero
- Emotional italic pull-quote with gold left border leads the content
- Mobile: dark overlay added so text stays readable against the grid background
- Launch → Grow → Succeed journey indicator (hidden on mobile for space)

### Carousel
- 6 slides: Businesses Launched, Turnaround Time, One-Stop Partner, Pricing, Data Recovery, Mobile-First
- **Auto-advances every 4 seconds** with a live gold progress bar
- Arrow buttons (left / right)
- Dot navigation — jumps to any page
- **Touch & swipe support** for mobile
- Pauses on hover (desktop)
- Responsive: 3 slides on desktop · 2 on tablet · 1 on mobile

### Interactive Package Builder
- 6 tickable services with individual from-prices
- Live running total updates instantly on every selection
- "Request This Package" CTA appears once at least one service is selected

### Quick Contact Widget
- 5 service category buttons
- Reveals a short form tailored to the selected service
- **Submits directly to WhatsApp** with service, name, and phone pre-filled

### Contact Form (Formspree)
- Endpoint: `https://formspree.io/f/mykqgdko`
- Fields: Name, Business Name, Phone, Service (dropdown), Message
- Green success message on send
- Red error message with phone number fallback if submission fails
- Form clears after successful submission
- Button disabled during submission to prevent duplicates

### Scroll Animations
- All sections fade and rise in as they enter the viewport
- Counter numbers animate from 0 to target on scroll-in

### WhatsApp Float Button
- Official WhatsApp SVG icon (not emoji) embedded inline
- Always visible, bottom-right corner
- Links to `https://wa.me/27820569497`

---

## Client Portfolio

| Client | Industry | Story |
|--------|----------|-------|
| **Sibani Trading Development Pty Ltd** | Trading & Development, Gauteng | Operating informally, losing tenders. ATHASH handled CIPC registration, SARS, logo, website and company profile. Submitted first formal tender within 3 weeks. |
| **Mbusi Cleaning Services** | Cleaning & Facilities, KwaZulu-Natal | Lost a corporate contract because they had no online presence. After website and branded email, won a 12-month corporate cleaning contract within 6 weeks. |
| **Confidential Accounting Firm** | Financial Services, Johannesburg | Hard drive failed mid-tax season. All data recovered in 18 hours, cloud backup configured. Now on monthly IT support retainer. |

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

To change the colour scheme, edit the `:root { }` block at the top of the `<style>` tag.

---

## Fonts

Loaded from Google Fonts with `preconnect` for faster rendering:

- **Montserrat** (400–900) — Headings, logo, buttons, labels
- **Inter** (300–600) — Body text, form fields

> Offline fallback: system sans-serif fonts.

---

## Contact Details in the Site

| Field | Value |
|-------|-------|
| Phone / WhatsApp | 082 056 9497 |
| Email | hello@athash.co.za |
| Website | www.athash.co.za |
| WhatsApp link | https://wa.me/27820569497 |
| Formspree form | https://formspree.io/f/mykqgdko |

To update any contact detail, search the HTML file for the current value and replace all instances.

---

## How to Deploy

### Option 1 — Direct upload (simplest)
Upload `athash-website-final.html` to any web host as `index.html`.

### Option 2 — GitHub Pages (free)
1. Create a GitHub repository
2. Upload the file renamed as `index.html`
3. Go to **Settings → Pages → Deploy from main branch**
4. Site is live at `https://yourusername.github.io/repo-name`

### Option 3 — Netlify (free, custom domain support)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop the HTML file onto the Netlify dashboard
3. Site is live in seconds — connect your domain in settings

### Option 4 — cPanel / shared hosting
1. Log into your hosting control panel
2. Open **File Manager → public_html**
3. Upload the file and rename it `index.html`

---

## How to Edit Common Things

| What to change | Where to find it |
|----------------|-----------------|
| Business name, phone, email | Search the file for the current value and replace |
| Hero headline or emotional line | Find `class="hero-h1"` and `class="hero-emotion"` |
| Pricing | Search for `R4,999`, `R2,999`, `R1,999` etc. |
| Stats numbers | Find `data-target="50"`, `data-target="30"`, `data-target="80"` |
| Portfolio stories | Find `<!-- PORTFOLIO -->` section |
| Testimonials | Find `<!-- TESTIMONIALS -->` section |
| Carousel slides | Find `<!-- CAROUSEL -->` and edit `.carousel-slide` blocks |
| Logo image | Replace `data:image/png;base64,...` in nav `<img>` tag |
| Founder photo | Replace `data:image/png;base64,...` in `.founder-avatar` `<img>` tag |
| Formspree endpoint | Search for `formspree.io/f/mykqgdko` |
| WhatsApp number | Search for `wa.me/27820569497` — replace number after `wa.me/` |
| Colour scheme | Edit CSS variables in `:root { }` at top of `<style>` block |
| Nav links | Find `<ul class="nav-links"` |

---

## Known Limitations

- **Google Fonts requires internet.** On first load with no connection, fallback system fonts show briefly.
- **Base64 images increase file size** to ~3MB. This is fine for most connections but may be slower on 2G. Consider hosting images separately and linking them if load speed becomes an issue.
- **Formspree free tier** allows 50 submissions/month. Upgrade at [formspree.io](https://formspree.io) if you exceed that.
- **IE 11 not supported** — CSS custom properties (variables) are not supported in Internet Explorer.

---

## Browser Support

| Browser | Support |
|---------|---------|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari (iOS & Mac) | ✅ Full |
| Samsung Internet | ✅ Full |
| Opera | ✅ Full |
| IE 11 | ❌ Not supported |

---

## Responsive Breakpoints

| Breakpoint | Layout |
|------------|--------|
| `> 1200px` | Full desktop — 3-column grids, carousel shows 3 slides |
| `961px – 1200px` | Medium — 2-column grids, carousel shows 2 slides |
| `≤ 960px` | Mobile — single column, hamburger nav, carousel 1 slide |

---

## Version History

| Version | File | Key Changes |
|---------|------|-------------|
| v1 | `athash-website.html` | Original uploaded file |
| v2 | `athash-website-v2.html` | Full redesign based on strategy critique |
| v3 | `athash-website-v3.html` | Real logo + founder photo embedded |
| v4 | `athash-website-v4.html` | Hamburger menu, carousel, hero gap fix |
| v5 | `athash-website-v5.html` | Real client stories, Formspree form, WhatsApp SVG icon |
| **Final** | `athash-website-final.html` | Favicon, font preconnect, emotional hero line, nav dropdown, carousel repositioned, stats softened, footer contact details, JS syntax fix |

---

## Credits

**Design & Development:** Built for ATHASH Digital Solutions
**Founder:** Snethemba Ngcobo
**Contact Form:** Formspree (`mykqgdko`)
**WhatsApp Icon:** Bootstrap Icons (MIT License)
**Fonts:** Google Fonts — Montserrat, Inter

---

*© 2025 ATHASH Digital Solutions. All rights reserved.*
