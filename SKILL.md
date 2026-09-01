---
name: interior-archive-print
description: Convert one interior photograph into a strict 3:4 split archival print poster with the untouched source photo above and a reference-locked illustrated reconstruction below. Use for Interior-Archive-Print requests; not for loose retro-poster styling.
---

# Interior Archive Print

This is a deterministic production workflow, not a loose style prompt.

## Required reading and authority

Before acting, read this file and the complete `REFERENCE.md`.

`REFERENCE.md` is the canonical, machine-readable visual specification in every runtime. It is never a fallback or a reduced-quality mode. If `reference/layout-reference.jpg` can truly be decoded and visually inspected, use it only to validate the interpretation of `REFERENCE.md`. If only its path, metadata, blob SHA, binary marker, or empty payload is available, record it internally as not visually inspected and continue without guessing. The JPG must never override hard constraints in `REFERENCE.md`.

- User photo = content truth: scene, architecture, viewpoint, furniture, objects, people, plants, lighting relationships.
- `REFERENCE.md` = visual truth: geometry, hierarchy, drawing language, ink, paper, color, typography, spacing.
- This file = process truth: analysis, generation, compositing, and rejection.

Never copy scene content or metadata from the reference image.

## Output contract

- Exactly one strict vertical 3:4 poster.
- Two equal-height zones separated by one perfectly straight horizontal boundary.
- Top: original uploaded photograph pixels. Proportional crop only.
- Bottom: generated reconstruction of the same scene and viewpoint, following `REFERENCE.md`.
- No overlap, feathering, torn edge, gradient, or element crossing the split.

The invariant is: **TOP = ORIGINAL PIXELS; BOTTOM = GENERATED INTERPRETATION.**

Never ask an image model to generate the complete poster. Generate only the lower artwork, then composite programmatically whenever a compositor is available. If exact pixel compositing is unavailable, do not claim strict completion; explain the limitation.

## Execution

### 1. Lock the visual system

Read all of `REFERENCE.md`. Use it as the authoritative interpretation and QC specification; it is not a prompt that should be copied mechanically into the image model. Keep its numeric ranges, hierarchy rules, color restrictions, typography limits, and failure tests available for validation. Do not reduce the intended system to generic words such as retro, vintage, editorial, Riso, or mid-century.

If the JPG is visually accessible, compare it against the specification for validation only. Never infer unseen details from its filename.

### 2. Lock the source

Inspect the uploaded photo and record:

- cropable region and camera direction/eye level;
- walls, openings, ceiling/floor direction, columns, beams, windows and perspective;
- hero furniture and major furniture count, silhouettes, segmentation and orientation;
- lamps, plants, artwork, shelving, audio objects and other scene anchors;
- foreground/middle/background, overlaps and occlusions;
- dominant light direction and one suitable muted accent color;
- only factual metadata explicitly supplied or visibly certain.

Never invent a city, building, designer, architect, brand, product model, date, or event.

### 3. Generate the lower panel only

Use the source lock for WHAT and `REFERENCE.md` for HOW. Preserve architecture, viewpoint, major object count and identity, positions, occlusions, and scene order. Small clutter may be grouped, but must not become new decor.

Use the concise generation instruction in section 11 of `REFERENCE.md`, supplemented only with source-specific facts from the source lock and, when necessary, one or two constraints addressing an observed failure. Do not paste every numeric target, QC test, or negative condition into the generation prompt. Detailed measurements and failure patterns belong to post-generation QC.

Before calling an image model, verify this generation gate internally:

- the requested output is the lower artwork only, never the complete poster;
- it reconstructs the uploaded scene from the same viewpoint;
- architecture, hero furniture, major object count, placement and depth order are locked;
- the medium is warm paper, brown-black hand-print linework and exactly one muted source-derived spot color;
- the drawing retains intentional paper exposure and contains no headline.

If any gate item is missing, repair the prompt before generation.

### 4. Composite

Create a 3:4 canvas. Crop the original source proportionally into the top half without regeneration, mirroring, stretching, object changes, or stylistic recoloring. Place the generated lower artwork in the bottom half. Keep all metadata in the lower zone and preserve the clean split.

### 5. Reject or deliver

Evaluate the generated lower panel against the complete `REFERENCE.md`. Reject and rebuild if any hard failure occurs. In particular, reject:

- any AI-generated or altered top panel;
- a cover-style headline, brand title, or `Daily Interior`-type display text;
- a generic magazine cover made from a large title plus polished architectural line art;
- a bottom panel that is edge-to-edge with no intentional paper;
- changed furniture count, viewpoint, architecture, or hero-object geometry;
- multicolor, photorealistic, CGI, watercolor, anime, clean-vector, or generic mid-century treatment;
- fabricated metadata.

## Final QC

Confirm all of the following before delivery:

- strict 3:4 and equal top/bottom geometry;
- top panel is traceably the original uploaded pixels;
- lower panel depicts the same scene, viewing direction, architecture, major furniture and anchors;
- lower artwork satisfies every relevant percentage and range in `REFERENCE.md`;
- warm paper, brown-black ink, exactly one muted spot color, controlled hatching and restrained print texture;
- metadata is tiny, compact and subordinate; no headline exists;
- intentional negative space remains;
- no invented facts or cross-boundary elements.

If any item fails, iterate before presenting the result.
