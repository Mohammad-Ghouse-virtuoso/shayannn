# Design System Document: The Living Heirloom

## 1. Overview & Creative North Star
**Creative North Star: "The Curated Artifact"**

This design system rejects the sterile, "app-like" interfaces of the modern web in favor of a tactile, editorial experience. It is designed to feel like a living heirloom—a private collection of memories held together by invisible threads. Instead of rigid grids and commercial components, we lean into **Intentional Asymmetry** and **Organic Layering**. 

The goal is to move away from "software" and toward "storytelling." We achieve this through:
*   **The Tonal Stack:** Using color shifts instead of lines to define space.
*   **The Found-Object Layout:** Elements should feel "placed" rather than "programmed," with subtle rotations and overlapping textures.
*   **The Ink & Parchment Contrast:** High-contrast serif typography paired with soft, textured backgrounds.

---

## 2. Colors & Surface Philosophy
The palette is rooted in nature and history, moving away from "digital" blues and vibrant notification reds.

### The Color Tokens
*   **Background / Surface:** `#fbf9f5` (A warm, aged parchment).
*   **Primary (Forest Green):** `#154212` – Use for the most important "ink" moments and heavy headers.
*   **Secondary (Dusty Gold):** `#7b5800` – Used for "brass" accents and special highlights.
*   **Tertiary (Ink Blue):** `#003091` – Used for subtle annotations and secondary "sketch" elements.

### The "No-Line" Rule
**Explicit Instruction:** 1px solid borders are strictly prohibited for sectioning. 
Boundaries must be defined by:
1.  **Tonal Shifts:** Placing a `surface-container-low` (#f5f3ef) element against a `surface` (#fbf9f5) background.
2.  **Negative Space:** Using the **Spacing Scale** (e.g., `12` or `16`) to let content breathe.
3.  **Organic Masks:** Using watercolor-edge masks rather than rectangular containers.

### Surface Hierarchy & Nesting
Treat the UI as a series of physical paper layers.
*   **Base:** `surface` (The desk).
*   **Layer 1:** `surface-container-low` (The journal page).
*   **Layer 2:** `surface-container-highest` (A taped-in photograph or a "scrap" of note paper).
*   **Floating Elements:** Use **Glassmorphism** (semi-transparent `surface-variant` with a 10px backdrop-blur) to simulate vellum or tracing paper overlays.

---

## 3. Typography
Typography is the "voice" of the journal. We pair the structured elegance of a serif with the warmth of a humanist touch.

*   **Display & Headlines (Epilogue):** This is our "Carved Ink." Use `display-lg` and `headline-lg` for section headers. The heavy weight creates an authoritative, editorial feel.
*   **Title & Body (Newsreader):** This is our "Handwritten Letter." The Newsreader serif provides a literary, classic quality. 
    *   Use `title-lg` for captions.
    *   Use `body-md` for long-form memories.
*   **The Human Touch:** For specific annotations or "scribbled" notes, override the system with a hand-drawn font (like Gaegu), but limit this to `label-md` or `title-sm` roles to maintain legibility.

---

## 4. Elevation & Depth
In this system, depth is **Ambient**, not mechanical.

*   **The Layering Principle:** Avoid CSS `box-shadow` on most items. Instead, stack `surface-container-lowest` (#ffffff) on top of `surface-container-high` (#eae8e4). The contrast alone creates the "lift."
*   **Ambient Shadows:** If an element must float (like a "pressed flower" or a "taped photo"), use an extra-diffused shadow: `rgba(27, 28, 26, 0.06)` with a 30px blur and 10px offset. This mimics natural, soft room light.
*   **The "Ghost Border":** For interactive inputs, use `outline-variant` (#c2c9bb) at **15% opacity**. It should be felt, not seen.
*   **Intentional Tilt:** Apply a slight rotation (between `-1deg` and `1.5deg`) to cards or "scraps" to break the digital grid.

---

## 5. Components

### The "Artifact" Button
*   **Primary:** Solid `primary` (#154212) with `on-primary` (#ffffff) text. No rounded corners (`none` or `sm`). It should look like a block-printed stamp.
*   **Tertiary:** No background. `title-sm` typography with a `secondary` (#7b5800) underline that looks like a hand-drawn ink stroke.

### Input Fields
*   **Styling:** Remove all background fills. Use a single bottom border (the "Ghost Border" at 20% opacity) to mimic a lined notebook.
*   **Focus State:** The bottom border shifts to `secondary` (Dusty Gold), and the label (using `label-md`) floats upward like a margin note.

### Chips (The "Taped Note")
*   Use `surface-container-highest`. 
*   **Corner Radius:** Use `none`. 
*   **Visual Flair:** Add a small `secondary-container` (#fdc34d) rectangle at the top center of the chip to simulate a piece of gold washi tape.

### Cards & Lists
*   **Strict Rule:** No dividers. Use **Spacing Scale 8 (2.75rem)** to separate list items.
*   **Cards:** Forbid the "white box with shadow" look. Use a `surface-container-low` background and an asymmetric padding (e.g., `pt-8 pb-12 px-6`) to make it feel like a hand-cut piece of paper.

### Signature Component: The "Ink Blot" Annotation
*   A decorative component used to highlight a specific word or image. It uses the `tertiary-container` (#0f45be) color in a low-opacity, organic SVG shape behind the text, simulating a spilled ink drop.

---

## 6. Do's and Don'ts

### Do:
*   **Embrace Asymmetry:** Offset images to the left or right; don't center-align everything.
*   **Use Watercolor Textures:** Apply a subtle grain or watercolor texture overlay to the `surface` background to break the flat hex color.
*   **Mix Type Sizes:** Use a very large `display-md` next to a very small `label-sm` to create high-end editorial drama.

### Don't:
*   **Don't use "Shiny" States:** Avoid gradients that imply plastic or glass (except for the vellum/blur effect).
*   **Don't use Standard Grids:** Avoid 12-column layouts that look like a storefront. Instead, use "staggered" columns where items are vertically offset.
*   **Don't use Pure Black:** Always use `on-surface` (#1b1c1a) for text. Pure black is too harsh for parchment.
*   **Don't use Icons for Everything:** Favor text labels or hand-drawn "sketches" over generic Material or FontAwesome icons.