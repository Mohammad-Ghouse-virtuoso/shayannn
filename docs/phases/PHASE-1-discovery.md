# Phase 1: Discovery

## Objective
Understand the current blueprint deeply enough to build without stylistic drift or unnecessary merge conflict.

## Scope
- Design extraction
- Section inventory
- Shared UI pattern inventory
- Risk and ambiguity capture

## Resources Selected
- `stitch_home_the_great_hall/stitch_home_the_great_hall/enchanted_journal/DESIGN.md`
- `stitch_home_the_great_hall/stitch_home_the_great_hall/my_story_home/code.html`
- `stitch_home_the_great_hall/stitch_home_the_great_hall/my_sketches_gallery/code.html`
- `stitch_home_the_great_hall/stitch_home_the_great_hall/my_treasures_toys/code.html`
- Workspace skills: `design-md`, `stitch-loop`, `enhance-prompt`

## Findings

### Design System Anchors
- Background is warm parchment with subtle texture.
- Main palette is forest green, dusty gold, and ink blue.
- Typography pairs strong editorial headlines with human handwritten notes.
- Composition relies on gentle rotation, taped edges, tonal layering, and asymmetry.
- Buttons and links behave like printed or handcrafted artifacts, not glossy UI controls.

### Shared Structural Patterns
- Every page has a top header with notebook branding and three main nav items.
- Every page has a footer with soft editorial styling.
- Every page embeds a full Tailwind config inline.
- Every page uses decorative scrapbook motifs: tape, paper layers, hand annotations, blurred blots.

### Cross-Page Implementation Needs
- Replace placeholder navigation with real links.
- Make header and footer behavior more consistent.
- Preserve page individuality while aligning interaction patterns.
- Review repeated token definitions for maintainability in a later phase.

## Risks
- Over-normalizing the pages could erase their handmade feel.
- Refactoring all repeated config too early could create noisy diffs.
- Branding rename decisions will affect all pages if changed later.

## Ambiguities
- Final public-facing site name.
- Whether to keep direct page-file editing or migrate to a cleaner public structure.

## Phase 1 Deliverables
- `SITE.md`
- `PLAN.md`
- `BUILD.md`
- `docs/sections/story-home.md`
- `docs/sections/sketches-gallery.md`
- `docs/sections/treasures-toys.md`

## Done Criteria
- Main pages are inventoried.
- Shared style rules are documented.
- Later phases have clear implementation targets.