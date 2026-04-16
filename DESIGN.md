# Ember Storytelling Page — Design Spec

## Overview

A scroll-driven interactive storytelling page for Ember, a halal smokehouse/BBQ brand. Sits alongside the main product site (embersmokery.co) as a standalone brand experience. The page sells the feeling of an Ember gathering — not the product itself.

## Target Audience

- Age 25-38, primarily hosts — people who organize dinners, parties, get-togethers
- New visitors who don't know Ember yet
- Secondary: existing fans and event planners

## Core Concept

"You Bring The People, We Bring The Smoke"

The page follows the arc of a gathering from the host's perspective. A scroll-driven lettuce-wrap animation serves as the visual spine — the lettuce unwraps with meat in the middle of the page, and wraps back up dropping into a person's mouth at the footer.

## Page Sections

### Section 1 — The Hook
- Full-screen lifestyle hero
- Photography: people gathering and eating, warm and energetic
- Bold headline (tone: "Every great night starts with someone saying 'come over.'")
- Scroll cue to pull user down

### Section 2 — The Popup (Engagement Moment)
- Triggered after initial scroll
- Soft overlay: "What are you planning?"
- 3-4 tappable visual cards: birthday / Friday night / family dinner / big party
- On selection: overlay closes, the next headline swaps to reflect choice (e.g. "Your birthday spread is about to be legendary" vs "Friday nights just got an upgrade")
- All other content stays the same — this is an engagement moment, not a content fork
- Keeps production and engineering simple

### Section 3 — The Unwrap (USP Moment)
- Scroll-driven animation: a real photo-cutout lettuce leaf opens up flat, meat lands on top
- This is the lettuce + meat USP moment — fresh meets smoky
- Minimal copy, something like "Fresh. Smoky. Always together."
- Mostly animation, not text — let the visual do the work

### Section 4 — The Moment
- Post-eating vibes: candid, warm photography
- People laughing, leaning back, in conversation
- Emotional peak of the page
- Copy like "This is what it's really about."
- Not posed — real energy

### Section 5 — The Ember Way
- Soft brand introduction
- Halal, smoked with care, made for sharing
- Not a hard sell — a quiet "this is who we are"
- One or two lines max
- Mascots (The Bear & The Dino) appear here

### Section 6 — The Wrap & Drop (Footer)
- Scroll-driven animation: the lettuce wraps back up around the meat and drops into a person's mouth
- Playful, satisfying, memorable
- Footer CTA: "Ready to host?" linking to embersmokery.co

## Scroll Animation Spine

The lettuce-wrap animation ties the page together:
- Section 3: Lettuce unwraps flat, meat lands on top (USP reveal)
- Sections 4-5: Storytelling content scrolls past
- Section 6: Lettuce wraps back up, drops into mouth (playful close)

The animation is built from **real photo cutouts** — lettuce and meat photographed separately on clean backgrounds, then layered and animated via scroll position. This keeps it on-brand (premium, tangible) rather than illustrated.

## Interactive Elements

- Scroll-triggered section animations (fade/slide in)
- Lettuce-wrap scroll animation (photo cutouts, parallax layers)
- One popup with occasion selection (engagement only, headline swap)
- Possible parallax on food photography sections
- Mascots as subtle recurring visual thread

## Photography Brief

The shoot team needs to deliver:

### Lifestyle Shots
1. **Hero gathering shot** — people eating together, warm energy, diverse group of 25-38 year olds (Section 1)
2. **Candid people moments** — post-eating, laughing, real interactions, not posed (Section 4)
3. **Closing/brand moment** — something clean for the Ember intro (Section 5)

### Product Cutout Assets (for scroll animation)
4. **Lettuce leaf** — single leaf, shot on clean/white background, top-down, high-res for animation
5. **Meat portion** — smoked meat, shot on clean/white background, top-down, matching angle to lettuce
6. **Person eating / mouth open** — for the footer drop moment, could be a fun candid shot

### Direction
- Halal context: no alcohol in any shots
- Warm lighting, nothing clinical or overly styled
- The host should be visible but not centered — the gathering is the star
- Diverse group, casual but elevated — not a backyard cookout, not a formal dinner, somewhere in between
- The food should look abundant and communal — platters, sharing, hands reaching

## Technical Notes

- Standalone site/page, separate from embersmokery.co
- Scroll-driven animations (GSAP ScrollTrigger or Framer Motion)
- Photo cutout animation: layered PNGs with scroll-position-driven transforms (rotation, scale, translate)
- Mobile-first design (primary audience will view on phones)
- Lightweight: mostly images, copy, and scroll triggers
- CTA links back to embersmokery.co for ordering

## Out of Scope (Future Projects)

- Sauce pairing interactive guide ("Build Your Plate" — pick meat, pick sauce, see combo)
- Product/menu page (already exists on embersmokery.co)
- E-commerce / ordering flow
