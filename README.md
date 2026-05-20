# Dubai Mall — Interactive Partner & Sponsorship Deck

> A cinematic, non-linear browser-based presentation deck built for Dubai Mall's commercial partnerships and leasing teams.

**[→ Live Demo]( [https://hakima-banoo.github.io/dubai-mall-deck])**

---

## Overview

This is a single-file interactive deck — not a website — built to communicate Dubai Mall's partnership and leasing opportunities to brands, sponsors, and retail partners. It mirrors the Digideck format: non-linear navigation, video-first storytelling, and luxury-grade UI inspired by brands like Apple, Hermès, and Tesla.

Dubai Mall is the world's most visited place on Earth (111M visitors in 2024), operated by Emaar Properties in Downtown Dubai adjacent to Burj Khalifa.

---

## Deck Structure (9 Slides)

| # | Slide | Content |
|---|-------|---------|
| 1 | **Hero** | Autoplay cinematic video · Real stats (111M visitors, 1,200+ stores, 13M sq ft) |
| 2 | **About** | Mall overview, key anchors, Fashion Avenue, expansion news |
| 3 | **Audience** | Animated demographic bars · 5 real metric cards with Emaar-sourced data |
| 4 | **Sponsorship Tiers** | Platinum / Gold / Select — AED-denominated with real benefit breakdowns |
| 5 | **Leasing** | Interactive zone tabs (Fashion Ave / Retail / F&B / Pop-Up) + clickable floor plan |
| 6 | **Attractions** | Dubai Aquarium, Dubai Fountain, Ice Rink, KidZania, Reel Cinemas, Burj Khalifa — with real photos |
| 7 | **Activations** | 4 proven formats: Takeovers, Digital OOH, Pop-Ups, Festival Co-Branding |
| 8 | **Events** | Cinematic video background · Dubai Shopping Festival, Food Festival, Super Sale |
| 9 | **CTA** | Meeting request · Emaar contact details |

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Framework | Vanilla HTML5 / CSS3 / JavaScript (ES6+) |
| Fonts | Google Fonts — Cormorant Garamond (display) + DM Sans (UI) |
| Video | Pexels royalty-free stock footage (embedded via `<video>`) |
| Images | Pexels royalty-free photography (CDN URLs, lazy-loaded) |
| Animations | CSS keyframes + JS-triggered scroll reveals |
| Navigation | Keyboard (←/→), scroll wheel, touch swipe, dot nav, module menu |
| Dependencies | **Zero** — no frameworks, no npm, no build step |
| Performance | Single file · ~46KB HTML · all media lazy-loaded · instant deploy |

---

## AI Tools Used

- **Claude (Anthropic)** — Architecture, all code generation, copywriting, data research, responsive CSS, interaction design
- **Perplexity / Claude web search** — Real-time verification of Dubai Mall visitor stats, occupancy rates, leasing rates, expansion details (Emaar sources, Time Out Dubai, Gulf Business)
- **Pexels AI search** — Sourcing royalty-free photography and video matched to each slide topic

All visitor data, retail counts, and financial figures are sourced from:
- Emaar Properties press releases (2024)
- Dubai Media Office official announcements
- Gulf Business, Time Out Dubai, Zawya (January 2025)

---

## Real Data Sources

| Metric | Value | Source |
|--------|-------|--------|
| Annual visitors 2024 | 111 million | Dubai Media Office / Emaar |
| YoY growth | +6% | Emaar H2 2024 release |
| Total area | 13M sq ft | Wikipedia / Emaar |
| Retail outlets | 1,200+ | Emaar |
| F&B outlets | 200+ | Emaar |
| Occupancy rate | 98% | Occupi / Emaar Q1 2025 |
| Rent growth | +24% YoY | Q3 2025 market reports |
| Retail sales growth H1 2024 | +8–15% | Emaar press release July 2024 |
| Customer satisfaction | 4.6/5 | Emaar / internal surveys |
| Instagram followers | 1.3M | Dubai Mall official account |
| Expansion budget | AED 1.5B | Emaar June 2024 announcement |

---

## Setup & Deployment

### Option 1 — Netlify Drop (30 seconds)
1. Go to [netlify.com/drop](https://netlify.com/drop)
2. Drag `index.html` onto the page
3. Get your live URL instantly

### Option 2 — Vercel (recommended for GitHub integration)
```bash
# 1. Create a GitHub repo and push this file
git init
git add .
git commit -m "Initial commit: Dubai Mall partner deck"
git remote add origin https://github.com/YOUR_USERNAME/dubai-mall-deck.git
git push -u origin main

# 2. Go to vercel.com → Import from GitHub → Deploy
# Your live URL will be: https://dubai-mall-deck.vercel.app
```

### Option 3 — GitHub Pages
1. Push `index.html` to a public GitHub repo
2. Settings → Pages → Source: main branch / root
3. Live at: `https://USERNAME.github.io/REPO-NAME`

---

## Design Decisions

**Why single-file?**
Portability and speed. No build step, no npm install, no CDN failures for JS dependencies. The evaluator can open it in any browser instantly.

**Why Cormorant Garamond + DM Sans?**
Cormorant reads as haute couture editorial — appropriate for a luxury destination pitch. DM Sans provides clean, legible UI contrast without competing for attention.

**Why dark luxury palette?**
Dark backgrounds with gold accents communicate premium positioning while making the photography and video feel cinematic rather than like stock-photo clutter.

**Non-linear navigation**
The module menu (left sidebar), dots (right), chapter-jump nav links, and keyboard/scroll/touch all work simultaneously. Viewers can jump directly to the section relevant to them (a sponsor skips to Tiers; a retailer jumps to Leasing).

**Video as primary medium**
Two video backgrounds (Hero + Events) autoplay silently. All other videos pause when off-screen for performance. Poster images ensure the slide is never blank.

---

## What I'd Improve With More Time

1. **Custom video production** — Commission or license actual Dubai Mall interior footage from Emaar's media library
2. **Micro-interactions** — Cursor trail on dark slides, parallax depth on the floor plan
3. **Analytics integration** — Track slide dwell time and CTA clicks for the sales team
4. **PDF export** — Generate a branded leave-behind from the live deck
5. **CMS layer** — Make tier pricing and availability editable without touching code
6. **More responsive breakpoints** — Dedicated mobile layout with vertical slide flow

---

## File Structure

```
/
├── index.html       ← Entire deck (HTML + CSS + JS in one file)
└── README.md        ← This file
```

---

*Built for the Liat AI take-home assignment. All content is for demonstration purposes. Dubai Mall is a trademark of Emaar Properties.*
