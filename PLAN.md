# Shayann Build Plan

## Goal
Build and refine the main pages from the existing Stitch blueprint in clear phases, using markdown as the planning and coordination layer.

## Main Pages
1. `site/index.html`
2. `site/sketches.html`
3. `site/treasures.html`

## Blueprint References
1. `my_story_home/code.html`
2. `my_sketches_gallery/code.html`
3. `my_treasures_toys/code.html`

## Phase Breakdown

### Phase 1. Discovery
Objective:
- Extract shared design anchors, page sections, reusable patterns, and implementation risks.

Resources:
- `enchanted_journal/DESIGN.md`
- Existing `code.html` files
- Future build target under `site/`
- `docs/sections/*.md`

Outputs:
- Section inventory markdown
- Shared style and implementation notes
- Open ambiguity list
- Clean target structure for implementation

### Phase 2. Shared Shell
Objective:
- Align header, navigation, footer, links, repeated tokens, and responsive rules across all pages.

Resources:
- `site/assets/styles.css`
- `site/index.html`
- `site/sketches.html`
- `site/treasures.html`
- All three blueprint `code.html` files for reference
- `docs/phases/PHASE-2-shared-shell.md`

Outputs:
- Unified navigation behavior
- Shared page conventions
- Reduced duplication where safe

### Phase 3. Story Home
Objective:
- Refine the home page as the main entry point and wire real navigation targets.

Resources:
- `my_story_home/code.html`
- `docs/sections/story-home.md`

Outputs:
- Stable home page structure
- CTA and quick-link behavior clarified

### Phase 4. Sketches Gallery
Objective:
- Refine scrapbook gallery composition, CTA behavior, and mobile navigation alignment.

Resources:
- `my_sketches_gallery/code.html`
- `docs/sections/sketches-gallery.md`

Outputs:
- Stable gallery layout
- Better content hierarchy and navigation consistency

### Phase 5. Treasures and Toys
Objective:
- Refine hero feature, card grid consistency, and narrative details.

Resources:
- `my_treasures_toys/code.html`
- `docs/sections/treasures-toys.md`

Outputs:
- Stable product-story hybrid page
- Consistent interaction patterns with other pages

### Phase 6. Responsive Polish
Objective:
- Validate and improve desktop, tablet, and mobile behavior across all pages.

Resources:
- All pages
- Browser validation

Outputs:
- Layout fixes
- Breakpoint consistency
- Navigation and spacing polish

### Phase 7. Handoff and Push Safety
Objective:
- Prepare the repo for low-conflict review and remote push.

Resources:
- Diff summary
- Phase markdown files

Outputs:
- Big-build checklist
- Review notes
- Clear next-step backlog

## Execution Notes
- Keep each phase scoped to the smallest meaningful review unit.
- Prefer direct edits only in files needed for that phase.
- Do not bundle unrelated visual or content changes.
- Treat blueprint files as design references unless explicitly asked to update them.