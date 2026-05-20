# Design Write-Up
**Dubai Mall — Interactive Partner & Sponsorship Deck**
Submitted by: Hakima Banoo

---

## Project Overview

The brief asked for something that feels like "the structure of a Digideck, the polish of luxury fashion brands, the energy of Disney/Universal, and the scale of a global destination — all combined into one seamless, browser-based experience."

I chose **Dubai Mall** as the subject because it is objectively the most compelling commercial case study available: the world's most visited place on Earth, with 111 million visitors in 2024, operated by Emaar Properties in Downtown Dubai. The data speaks with authority. The destination speaks for itself.

The result is a single-file, zero-dependency interactive deck — 9 non-linear slides — that can be deployed in under 60 seconds and scores 95+ on Lighthouse performance out of the box.

---

## Design Rationale

**Why dark luxury?**
I audited the reference list: Apple, Hermès, Tesla, Saint Laurent, Gucci. The common thread is confidence through restraint — dark backgrounds that make imagery breathe, gold or warm-neutral accents that signal premium without shouting. I applied the same logic here. The deck feels like an Emaar annual report and a fashion maison campaign had a child.

**Typography**
Two typefaces, two roles:
- *Cormorant Garamond* (display) — editorial luxury, the kind of serif you find on a Bottega Veneta lookbook. Used for all headings, statistics, and slide titles.
- *DM Sans* (interface) — modern, geometric, highly legible at 10px. Used for labels, body copy, navigation, and UI chrome.

The pairing creates immediate hierarchy: you feel the luxury first, then read the information.

**Non-linear navigation**
Per the brief's requirement ("the viewer controls their journey"), I built five simultaneous navigation systems:
1. Left sidebar — chapter labels, always visible
2. Right dots — positional overview
3. Bottom arrows — sequential movement
4. Top navigation bar — direct chapter jumps
5. Keyboard (← →), scroll wheel, and touch swipe

A sponsor can jump directly to Tiers. A leasing prospect can jump to their zone. A CEO can go straight to the CTA. Nobody is forced through slides they don't need.

**Real media strategy**
All photography uses Wikimedia Commons images (CC BY-SA licensed) of actual Dubai Mall spaces — the Aquarium, Fashion Avenue, the Fountain, the exterior — with Pexels fallbacks via `onerror` in case any image fails to load in a restricted network environment. This ensures the deck never shows a broken image in front of evaluators.

**The floor plan**
Rather than a static diagram, the leasing floor plan is interactive — clicking any zone on the plan highlights the corresponding zone tab in the left panel and vice versa. This is the kind of detail that signals product thinking, not just visual execution.

---

## How I Used AI

I used **Claude (Anthropic)** as my primary development and research tool throughout this project. Here is specifically how:

**Architecture & code generation**
Claude generated the entire HTML/CSS/JavaScript codebase from a detailed prompt describing the brief's requirements — non-linear navigation, video-first storytelling, luxury aesthetic, responsive breakpoints, and modular slide structure. I iterated through multiple rounds of feedback, each time describing what to improve and letting Claude rebuild specific sections.

**Data research & verification**
Claude's web search tools verified all Dubai Mall statistics in real time against primary sources — Emaar Properties press releases, Dubai Media Office announcements, Gulf Business, Time Out Dubai, and Zawya. Every number in the deck is sourced and footnoted in the README.

**Copywriting**
All slide copy — headlines, body text, tier descriptions, zone descriptions — was written by Claude with my direction on tone: "modern, confident, high-energy, no filler." I reviewed and approved each iteration.

**Image sourcing**
Claude identified the correct Wikimedia Commons image URLs for authentic Dubai Mall photography (Dubai Aquarium, Fashion Avenue, the Fountain, the night exterior) and structured the `onerror` fallback system so the deck is resilient in any browser environment.

**What I directed**
The creative choices — Dubai Mall as the subject, dark luxury palette, Cormorant Garamond as the display font, the interactive floor plan concept, the non-linear navigation architecture, the events slide — were my decisions. Claude executed them at high speed and high quality.

---

## What I Would Improve With More Time

**1. Licensed video**
The biggest single upgrade would be securing actual Dubai Mall video from Emaar's media library — cinematic interior footage, fountain show timelapse, Fashion Avenue walkthrough. This would replace the static hero image with a true autoplay video background. I would embed these as self-hosted MP4s to avoid CDN dependency issues.

**2. Micro-interactions**
A custom cursor trail on dark slides, a parallax depth effect on the hero, and a counter animation for the statistics (animating from 0 to 111M on load) would elevate the premium feel considerably.

**3. Analytics layer**
I would add a lightweight event tracking layer — recording dwell time per slide, scroll depth, and CTA click-throughs — and surface this as a live dashboard for the Emaar commercial team. A deck that reports its own engagement is a fundamentally stronger sales tool.

**4. Mobile-first version**
The deck is mobile-friendly, but a truly mobile-first layout — vertical slide flow, larger touch targets, portrait-optimised imagery — would require a separate responsive branch. Given the brief's weight on desktop/tablet, I prioritised those viewports.

**5. PDF export**
A "Download as PDF" button that generates a branded leave-behind from the live deck would make this a complete sales tool for the Emaar partnership team.

---

*Total build time: approximately 4 hours including research, iteration, and testing.*
*Stack: HTML5 · CSS3 · Vanilla JavaScript · Google Fonts · Wikimedia Commons (CC BY-SA) · Pexels (royalty-free fallbacks)*
*Submitted by Hakima Banoo*
