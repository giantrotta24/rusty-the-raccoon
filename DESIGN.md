---
name: Rusty the Raccoon
description: Companion site for Michelle Trotta's picture book — warm night teal, cream pages, and firefly glow.
colors:
  teal: "#144c53"
  teal-deep: "#0c3339"
  teal-tint: "#1f6b74"
  cream: "#f7f3ea"
  cream-soft: "#fffdf9"
  amber: "#f2a93b"
  amber-deep: "#d3860f"
  coral: "#ef6f63"
  coral-ink: "#b8453c"
  slate: "#66759a"
  slate-ink: "#4a5670"
  ink: "#1e2e30"
  white: "#ffffff"
typography:
  display:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "clamp(2.2rem, 4.5vw, 3.4rem)"
    fontWeight: 700
    lineHeight: 1.15
  headline:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "clamp(1.6rem, 3vw, 2.3rem)"
    fontWeight: 600
    lineHeight: 1.15
  title:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "1.3rem"
    fontWeight: 600
    lineHeight: 1.15
  title-sm:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "1.2rem"
    fontWeight: 600
    lineHeight: 1.15
  body:
    fontFamily: "'Nunito Sans', 'Segoe UI', sans-serif"
    fontSize: "1.05rem"
    fontWeight: 400
    lineHeight: 1.65
  body-sm:
    fontFamily: "'Nunito Sans', 'Segoe UI', sans-serif"
    fontSize: "0.95rem"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "0.85rem"
    fontWeight: 600
    letterSpacing: "0.06em"
  brand:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "1.45rem"
    fontWeight: 700
    letterSpacing: "0.09em"
  brand-sm:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "clamp(0.78rem, 4vw, 1.02rem)"
    fontWeight: 700
  byline:
    fontFamily: "Caveat, cursive"
    fontSize: "1.5rem"
    fontWeight: 600
  byline-sm:
    fontFamily: "Caveat, cursive"
    fontSize: "clamp(0.9rem, 4.4vw, 1.15rem)"
    fontWeight: 600
  script:
    fontFamily: "Caveat, cursive"
    fontSize: "1.9rem"
    fontWeight: 600
    lineHeight: 1.1
  script-sm:
    fontFamily: "Caveat, cursive"
    fontSize: "1.75rem"
    fontWeight: 600
  credit:
    fontFamily: "'Nunito Sans', 'Segoe UI', sans-serif"
    fontSize: "0.75rem"
    fontWeight: 400
  nav:
    fontFamily: "'Nunito Sans', 'Segoe UI', sans-serif"
    fontSize: "0.95rem"
    fontWeight: 700
  publisher:
    fontFamily: "Fredoka, 'Baloo 2', sans-serif"
    fontSize: "1.15rem"
    fontWeight: 600
rounded:
  xs: "2px"
  focus: "4px"
  sm: "10px"
  md: "18px"
  lg: "28px"
  pill: "999px"
spacing:
  wrap-inline: "1.5rem"
  section-block: "clamp(3rem, 7vw, 5.5rem)"
  max-width: "1160px"
components:
  button-teal:
    backgroundColor: "{colors.teal}"
    textColor: "{colors.white}"
    rounded: "{rounded.pill}"
    padding: "0.85em 1.7em"
    typography: "{typography.display}"
  button-amber:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.teal-deep}"
    rounded: "{rounded.pill}"
    padding: "0.85em 1.7em"
    typography: "{typography.display}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.teal}"
    rounded: "{rounded.pill}"
    padding: "0.85em 1.7em"
  card:
    backgroundColor: "{colors.cream-soft}"
    rounded: "{rounded.md}"
    padding: "1.75rem"
  section-teal:
    backgroundColor: "{colors.teal}"
    textColor: "{colors.cream-soft}"
---

# Design System: Rusty the Raccoon

## Overview

**Creative North Star: "The Firefly Jar"**

The site feels like carrying a jar of fireflies through a New York night — deep teal “night” bands, cream daylight pages, and soft amber points that echo Rusty and Squeaks’ glowing jar. Book artwork leads; UI stays supportive, rounded, and kid-friendly without talking down to the adults who buy, download, and teach.

Tokens live in `src/styles/global.css`. Light-only; no dark theme. Visual anti-references: generic SaaS purple gradients, thick left-border “AI cards,” and inventing substitute brand art.

**Key Characteristics:**
- Book cover and Alisha Uguccini illustrations as the authority
- Teal night sections with decorative fireflies (`aria-hidden`)
- Cream page fields with dashed coral accents on activity/resource cards
- Fredoka display + Nunito Sans body + Caveat for warm asides
- Pill buttons; soft teal-tinted shadows; 780px / 640px grid breakpoints

## Colors

Night teal and paper cream are sampled from the original site; amber/coral come from the book’s firefly glow and confetti accents.

### Primary
- **Night Teal** (`#144c53`): Section backgrounds, headings on cream, primary buttons, focus rings on light surfaces
- **Teal Deep** (`#0c3339`): Gradient bottoms, amber-button text, deeper hover

### Secondary
- **Firefly Amber** (`#f2a93b`): Glow motif, CTAs that need warmth, focus rings on teal surfaces
- **Amber Deep** (`#d3860f`): Amber button hover

### Tertiary
- **Coral** (`#ef6f63`): Decorative dashes and accents only
- **Coral Ink** (`#b8453c`): Text/labels on cream (AA)

### Neutral
- **Cream** (`#f7f3ea`): Page background
- **Cream Soft** (`#fffdf9`): Cards, soft text on teal
- **Ink** (`#1e2e30`): Body text
- **Slate Ink** (`#4a5670`): Secondary body (credits); prefer over bright slate for text
- **White** (`#ffffff`): Headings on teal, solid fills

### Named Rules
**The Glow-Not-Paint Rule.** Amber is light in the dark — fireflies, focus on teal, warm CTAs — not a blanket brand wash.

**The Bright-Is-Decoration Rule.** Raw coral and slate are for accents; text uses `coral-ink` / `slate-ink` / ink / teal.

## Typography

**Display Font:** Fredoka (self-hosted `@fontsource`)
**Body Font:** Nunito Sans
**Script Font:** Caveat (hero asides, author byline)

**Character:** Rounded, friendly, readable for parents and therapists; script only for short warm prompts.

### Hierarchy
- **Display** (700, `clamp(2.2rem, 4.5vw, 3.4rem)`): Page heroes
- **Headline** (600, `clamp(1.6rem, 3vw, 2.3rem)`): Section titles
- **Title** (600, ~1.3rem): Card titles
- **Body** (400, 1.05rem / 1.65): Prose; keep measure near 60–65ch where constrained
- **Script** (600): Short CTAs and bylines — never long paragraphs

## Layout

Centered `.wrap` at `max-width: 1160px` with `1.5rem` inline padding. Sections use `clamp(3rem, 7vw, 5.5rem)` vertical rhythm. Content grids: 2-col from 640px, 3-col from 780px; hero splits at 780px. Mobile header switches at 820px (disclosure menu, peeking Rusty logo). Sticky footer via `min-height: 100dvh` flex column on `body`.

## Elevation & Depth

Soft teal-tinted shadows, not hard offsets. Lift on hover (translate + shadow), not resting neon glow.

### Shadow Vocabulary
- **Soft** (`0 4px 16px -6px rgba(20, 76, 83, 0.18)`): Cards at rest
- **Card** (`0 10px 30px -12px rgba(20, 76, 83, 0.25)`): Hero art, hover elevation
- **Amber bloom** (button hover): intentional firefly-adjacent glow on amber CTAs only

## Shapes

Generous radii: `10 / 18 / 28px` plus full pills for buttons and nav chips. Activity/resource cards share a **dashed coral top rule** — not a thick left border. Circles for social icons and contact badge.

## Components

### Buttons
Pill Fredoka labels. Variants: `btn-teal`, `btn-amber`, `btn-outline`. Hover lifts slightly (`translateY(-2px)`).

### Cards
Cream-soft surface, soft shadow, dashed coral top accent for activity and resource grids.

### Navigation
Desktop pill links with `min-height: 44px`; current page fills teal. Mobile: zero-JS `<details>` menu.

### Teal night section
Gradient teal → teal-deep, cream/white type, optional `.firefly-field` (decorative, `aria-hidden`).

### Focus
Teal outline on cream surfaces; amber outline inside `.section-teal`. Always `focus-visible`, 3px / 3px offset.

## Do's and Don'ts

### Do
- Lead with real book and character art
- Keep free activities and resources easy to find
- Use fireflies only on teal night bands
- Prefer tokens from `:root` over one-off hex
- Name download controls with the activity title for assistive tech

### Don't
- Invent brand art, testimonials, or series titles
- Use thick colored left borders on cards
- Put bright coral/slate on body copy
- Globally nuke transitions under `prefers-reduced-motion` — only pause decorative fireflies
- Build a dark theme unless product asks for it
