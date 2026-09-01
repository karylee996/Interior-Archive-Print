---
name: Interior-Archive-Print
description: Strict reference-locked workflow for turning one interior photograph into a 3:4 vertical split poster: exact original photo on top, archival print reconstruction below, visually anchored to reference/layout-reference.jpg.
---

# Interior-Archive-Print

## READ FIRST — THIS IS A REFERENCE-LOCKED SKILL

This is NOT a loose style prompt and must not be executed from the repository name alone.

The repository contains one canonical visual reference:

`reference/layout-reference.jpg`

That image is the GOLD STANDARD for the visual result. It simultaneously defines layout character, illustration language, print texture, palette restraint, typography scale, spacing, negative space, and overall editorial atmosphere.

### Three sources have different authority

**USER SOURCE PHOTO = CONTENT TRUTH**
Controls architecture, viewpoint, furniture identity/count, object placement, people, plants, lighting relationships, and scene content.

**reference/layout-reference.jpg = VISUAL TRUTH**
Controls visual treatment, printmaking character, graphic hierarchy, illustration abstraction level, line density, color restraint, paper feeling, typography behavior, spacing, and editorial mood.

**SKILL.md = EXECUTION TRUTH**
Controls the workflow and prevents improvisation.

Never borrow furniture, architecture, people, plants, objects, or factual metadata from the reference image. Never borrow the source photo's photographic rendering style for the lower panel. Content comes from the user photo; visual grammar comes from the canonical reference.

---

## NON-NEGOTIABLE STARTUP SEQUENCE

When invoked in any chat, especially a new chat, execute in this order BEFORE generating:

1. Retrieve and read the COMPLETE `SKILL.md`.
2. Retrieve and visually inspect `reference/layout-reference.jpg`.
3. Analyze the canonical reference as a visual system, not merely by filename.
4. Inspect the user's uploaded source photo.
5. Separate CONTENT constraints from STYLE constraints.
6. Generate ONLY the lower archival interpretation, using BOTH the user photo and canonical reference with their separate roles.
7. Preserve the user's original photograph pixels for the upper panel.
8. Composite the two panels into the final strict 3:4 poster.
9. Run Final QC.

If `reference/layout-reference.jpg` cannot actually be accessed as a visual image, DO NOT pretend it was inspected. Use the written Visual DNA below as fallback and, where possible, retrieve the reference through a method that exposes the image visually.

Do not generate merely because the repository name sounds descriptive.
Do not summarize this file and then improvise.
Do not replace the reference with a generic interpretation of “retro”.

---

## REFERENCE LOCK — WHAT TO LEARN FROM THE CANONICAL IMAGE

Before each generation, visually inspect the reference and lock these dimensions:

- exact overall upper/lower hierarchy;
- relative amount of image versus paper/negative space;
- illustration scale within the lower panel;
- line thickness and irregularity;
- hatching density and direction;
- shadow abstraction level;
- ratio of unprinted paper to printed ink;
- spot-color coverage;
- paper warmth;
- ink softness/density;
- degree of print imperfection;
- typography size relative to canvas;
- typography alignment and placement;
- spacing between illustration and metadata;
- overall editorial quietness.

Do NOT copy scene-specific content from the reference.

The goal is not pixel duplication. The goal is to transfer its DESIGN GRAMMAR to a new scene.

---

## WRITTEN VISUAL DNA — FALLBACK AND REINFORCEMENT

The canonical reference should be interpreted through the following stable visual DNA:

### Editorial character

A premium found-page feeling from a 1970s–1980s interior design archive, architecture journal, independent furniture catalogue, museum-shop publication, or carefully art-directed design annual.

Quiet, observational, restrained, tactile, intelligent. Not a commercial advertising poster.

### Print language

- hand-drawn architectural ink character;
- linocut / woodcut / wood engraving influence;
- screen-print and Risograph behavior;
- irregular dark brown-black outlines;
- parallel hatching and cross-hatching;
- selective solid ink masses;
- sparse halftone;
- subtle broken/dry ink;
- mild registration imperfection;
- physical print character without excessive grunge.

### Paper

- warm ivory / cream;
- uncoated stock feeling;
- visible but restrained fiber/grain;
- never sterile digital white;
- never heavily yellowed antique parchment.

### Color

Use a deliberately limited system:

1. warm cream paper;
2. deep brown-black / softened black structural ink;
3. ONE principal muted spot color derived from the USER SOURCE PHOTO.

The spot color is selective, not full-scene coloring. Large areas should remain paper or dark linework.

Examples: greenery → olive/moss; red furniture/art → brick/oxblood; caramel leather/timber → tobacco/burnt orange; blue feature → muted slate/navy.

### Illustration abstraction

The lower illustration must sit between technical observation and handmade printmaking. It must remain spatially recognizable but should not chase photographic detail.

Preserve major silhouettes and relationships; translate surfaces and shadows into hatching, ink masses, sparse color, and negative paper.

### Typography

- very small;
- monospaced/typewriter/technical archive character;
- quiet, secondary, never headline-dominant;
- aligned deliberately within a simple grid;
- generous breathing room;
- archival number + short keywords + optional known date/location + short observational microcopy.

No fake sophistication through invented facts.

---

## OUTPUT CONTRACT

Final result:

- exactly ONE independent poster;
- strict vertical 3:4 aspect ratio;
- upper visual zone approximately 50%;
- lower visual zone approximately 50%;
- clean straight horizontal division;
- no collage behavior;
- no decorative object crossing the split.

### TOP = ORIGINAL PIXELS

The upper panel must use the actual uploaded source photograph.

Allowed: proportional crop to fit.

Forbidden: AI redraw, regeneration, mirroring, stretching, moving objects, changing architecture, adding/removing people/furniture, replacing materials, changing products, stylistic recoloring.

### BOTTOM = REFERENCE-LOCKED INTERPRETATION

The lower panel depicts the SAME source scene from the SAME viewing direction but translated through the visual grammar of `reference/layout-reference.jpg`.

---

## MANDATORY WORKFLOW

### PASS A — ANALYZE CANONICAL REFERENCE

Silently determine its:

- visual hierarchy;
- layout rhythm;
- illustration-to-paper ratio;
- print density;
- line language;
- hatching language;
- color coverage;
- typography scale;
- whitespace behavior;
- texture strength;
- overall degree of abstraction.

These become STYLE LOCKS.

### PASS B — ANALYZE USER SOURCE PHOTO

Identify:

- room/scene type;
- camera angle and eye level;
- architectural structure;
- hero furniture/object;
- major furniture count;
- furniture silhouettes;
- lamps;
- plants;
- artwork;
- shelving/audio/objects where relevant;
- foreground/middle/background;
- major overlaps and occlusions;
- lighting direction;
- one scene-representative accent color;
- only factual metadata actually supplied or reliably known.

These become CONTENT LOCKS.

### PASS C — GENERATE LOWER PANEL ONLY

Use the user photo for CONTENT LOCKS and `reference/layout-reference.jpg` for STYLE LOCKS.

The lower image must preserve:

- source architecture;
- source viewpoint;
- source furniture identity/count;
- source object positions;
- source foreground/background relationships;
- source major silhouettes;
- source scene identity.

But its rendering must follow the canonical reference's visual grammar.

Do not ask the image model to generate the entire top+bottom poster in one pass.

### PASS D — COMPOSITE

Create the strict vertical 3:4 canvas programmatically when an image compositor is available.

- Place ORIGINAL uploaded photograph in upper ~50%.
- Crop proportionally; never stretch.
- Place generated lower artwork in lower ~50%.
- Use a straight clean boundary.
- Keep typography inside the lower panel.
- Do not allow lower artwork to overlap the source photograph.

This compositing stage is mandatory because text instructions such as “preserve the photo” do not guarantee that an image generator will retain original pixels.

---

## FIDELITY PRIORITY

If style and content conflict, source-scene fidelity wins for WHAT is depicted; reference fidelity wins for HOW it is depicted.

Content priority:
1. architecture;
2. viewpoint;
3. furniture count;
4. furniture identity;
5. object placement;
6. foreground/background order.

Style priority:
1. canonical layout hierarchy;
2. line/hatching character;
3. abstraction level;
4. paper/ink relationship;
5. limited color behavior;
6. print texture;
7. typography scale and spacing.

Never redesign the user's room to resemble the reference room.

---

## TYPOGRAPHY SYSTEM

Use small archival metadata only.

Typical structure:

`No. 041`

`retro corner / warm light / objects and posters`

`20XX` only if an actual year is known or a clearly neutral placeholder is appropriate.

One short observational sentence may follow.

Language is adaptive. Do not force Korean, Japanese, Chinese, or English. Do not infer a location from aesthetic cues.

Never invent city, country, architect, designer, product name, date, or event.

---

## NEGATIVE CONSTRAINTS

Do NOT allow the lower panel to drift into:

- generic “retro poster” styling;
- flat clean vector art;
- watercolor;
- anime/cartoon;
- glossy 3D/CGI;
- photorealistic redraw;
- luxury interior redesign;
- Bauhaus geometry unrelated to the reference;
- scrapbook collage;
- random stickers/stamps/arrows;
- vivid multicolor illustration;
- excessive distressed/grunge paper;
- fantasy architecture;
- added decorative objects;
- oversized advertising headlines.

Do NOT copy scene content from the canonical reference.

---

## SCENE ADAPTATION

### Furniture-led
Preserve upholstery geometry, arm shape, legs/base, cushion segmentation, and relation to adjacent objects. Allow the scene-derived spot color to emphasize the hero furniture when appropriate.

### Architecture-led
Prioritize openings, walls, columns, windows, stairs, ceiling rhythm, floor geometry, and perspective relationships.

### Plant-heavy
Preserve major plant silhouettes and placement. Simplify leaves into grouped engraved masses. Olive/moss may become the spot color when visually justified.

### Object-rich / retro
Preserve recognizable anchor objects such as speakers, record players, clocks, lamps, books, framed art, radios, globes, and shelving. Tiny secondary clutter may be graphically grouped.

### Minimal
Do not fill empty areas with unnecessary hatching. Match the canonical reference's restraint and allow paper to breathe.

---

## FINAL QC — REFERENCE COMPARISON IS MANDATORY

Before output, compare the result against BOTH inputs.

### Against user source photo

- [ ] same scene identity;
- [ ] same viewing direction;
- [ ] architecture corresponds;
- [ ] major furniture count corresponds;
- [ ] hero furniture remains recognizable;
- [ ] major object positions correspond;
- [ ] nothing important was invented, removed, mirrored, or redesigned.

### Against canonical reference

- [ ] lower panel feels like the same design family;
- [ ] line density is comparable;
- [ ] hatching language is comparable;
- [ ] abstraction level is comparable;
- [ ] paper warmth is comparable;
- [ ] dark ink behavior is comparable;
- [ ] spot-color restraint is comparable;
- [ ] print texture strength is comparable;
- [ ] typography is similarly small and quiet;
- [ ] negative-space behavior is comparable;
- [ ] overall result feels editorial rather than template-like.

### Final format

- [ ] strict vertical 3:4;
- [ ] upper/lower approximately 1:1;
- [ ] upper panel contains original photo pixels;
- [ ] straight split;
- [ ] no cross-boundary graphics;
- [ ] no fabricated metadata.

If the lower panel matches the words in SKILL.md but visibly does NOT belong to the same design family as `reference/layout-reference.jpg`, it FAILS and should be regenerated.

If the upper panel was regenerated instead of using original pixels, it FAILS and must be rebuilt by compositing the original photo.

---

## NEW-CHAT INVOCATION RULE

When the user says, for example:

“读取并严格执行 GitHub 上 karylee996/Interior-Archive-Print 的完整 SKILL.md，按这个 Skill 生成我上传的照片。”

The assistant must first retrieve:

1. `SKILL.md`
2. `reference/layout-reference.jpg`

Only then may it generate.

The assistant must treat the reference image as a REQUIRED VISUAL INPUT, not an optional example or a filename mentioned in prose.

**Source photo determines WHAT. Canonical reference determines HOW. SKILL.md determines PROCESS.**
