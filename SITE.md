# Shayann Site Build Map

## 1. Purpose
This file is the top-level coordination map for building the Shayann website from the existing Stitch blueprint pages while keeping the visual language coherent and merge-safe.

## 2. Current Assumptions
- The current `code.html` files are visual blueprints, not the implementation target.
- The existing design language in `enchanted_journal/DESIGN.md` is the source of truth for style decisions.
- We will build a cleaner site structure under `site/` and use the blueprints as reference only.
- Desktop quality comes first, but every phase must preserve tablet and mobile support.

## 3. Design Source
- Primary design reference: `stitch_home_the_great_hall/stitch_home_the_great_hall/enchanted_journal/DESIGN.md`

## 4. Active Pages
- Blueprint: `my_story_home/code.html`: Home and story-led landing page.
- Blueprint: `my_sketches_gallery/code.html`: Sketchbook gallery page.
- Blueprint: `my_treasures_toys/code.html`: Toys and treasures collection page.
- Build target: `site/index.html`
- Build target: `site/sketches.html`
- Build target: `site/treasures.html`

## 5. Shared Style Anchors
- Warm parchment background and tonal paper layering.
- Deep green primary, dusty gold secondary, ink-blue tertiary accents.
- Editorial serif plus playful hand-drawn annotations.
- Asymmetric scrapbook composition, taped elements, tilted cards, watercolor texture.
- Soft ambient depth instead of hard UI chrome.

## 6. Phase Roadmap
- Phase 1: Discovery and implementation map.
- Phase 2: Shared shell and navigation system.
- Phase 3: Story Home build and cleanup.
- Phase 4: Sketches Gallery build and cleanup.
- Phase 5: Treasures and Toys build and cleanup.
- Phase 6: Responsive and interaction polish.
- Phase 7: Final QA, handoff, and push-safe review.

## 7. Open Questions
- Branding is confirmed as `Shayann`.
- Implementation is confirmed to live in a new consolidated `site/` structure.

## 8. Working Rule
For medium and large work, update the relevant phase file before implementation and summarize the result after implementation.