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

## Photography Brief & Shot List

The shoot team needs to deliver the following. Products on table: sauces, sides, smoked meat, lettuce wraps.

### Shot 1 — Hero Table Spread (Section 1)
**The Gathering Table — wide angle**
- Overhead or 45-degree angle of a full table spread
- Meat platters, sides in bowls, sauces lined up, lettuce wraps being assembled
- 4-6 people's hands reaching in, passing plates
- Warm lighting, not flash — think golden hour or warm indoor
- The table should feel abundant but not messy
- Sauces should be visible on the table even if not the focus — builds familiarity before they hit the product site

### Shot 2 — Candid People Moments (Section 4)
**3-4 setups needed:**
- **The laugh** — someone mid-laugh with food in hand, others reacting
- **The pass** — two people sharing a plate or passing a wrap across the table
- **The lean-back** — post-eating, satisfied, still talking, plates half-finished
- **The build** — someone assembling a lettuce wrap (meat + sauce), hands in focus

### Shot 3 — Product Cutouts (Section 3 & 6 — scroll animation)
**Shot on clean white/light background, top-down:**
- Single lettuce leaf — flat, fully open, high-res
- Smoked meat portion — sitting naturally, matching scale to the lettuce
- A wrapped lettuce + meat combo — for the "wrap" animation at footer
- Individual sauces in small bowls — top-down, for potential secondary use

### Shot 4 — Brand / Closing (Section 5 & 6)
- **The aftermath** — a table post-meal, plates scattered, people still there, warm and lived-in
- Or **the mascot moment** — if incorporating Bear & Dino physically (plushies, stickers on the table, printed on packaging visible in shot)

### General Direction
- **No alcohol** in any frame
- **Diverse group, 25-35 age range**, casual but put-together
- **Warm tones** — golden, amber, not blue/cool
- **Nothing posed** — if it looks like a stock photo, reshoot it
- Shoot **horizontal for desktop, vertical crops for mobile** — or shoot wide enough to crop both ways
- The host should be visible but not centered — the gathering is the star
- Casual but elevated — not a backyard cookout, not a formal dinner, somewhere in between

### Priority
The most important shots are the **hero table spread** (Shot 1) and the **product cutouts** (Shot 3) — those carry the whole page. Everything else supports the mood.

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
