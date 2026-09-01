---
name: Interior-Archive-Print
description: Strict reference-locked workflow for turning one interior photograph into a 3:4 vertical split poster: exact original photo on top, archival print reconstruction below.
---

# Interior-Archive-Print

## READ FIRST — REQUIRED FILES

This is NOT a loose style prompt. Before generating anything, retrieve and read:

1. the COMPLETE `SKILL.md`;
2. the COMPLETE `REFERENCE.md`;
3. `reference/layout-reference.jpg` if the runtime can actually expose it as a visual image.

IMPORTANT: GitHub access may expose the JPG only as binary metadata and not as viewable pixels. If the JPG cannot actually be visually inspected, DO NOT pretend to have seen it. In that case, `REFERENCE.md` is the authoritative textual replacement.

Never execute this Skill from the repository name alone.

## AUTHORITY MODEL

**USER SOURCE PHOTO = CONTENT TRUTH / WHAT**
Architecture, viewpoint, furniture identity/count, objects, people, plants, spatial relationships, lighting relationships, scene content.

**layout-reference.jpg OR REFERENCE.md = VISUAL TRUTH / HOW**
Layout character, illustration language, printmaking character, line density, hatching, abstraction, paper, ink, spot-color behavior, typography scale, spacing, negative space, editorial atmosphere.

**SKILL.md = EXECUTION TRUTH / PROCESS**
Workflow, separation of generation and compositing, fidelity rules, and QC.

Never copy furniture, architecture, objects, people, plants, or factual metadata from the canonical reference. The source photo determines content; the reference system determines rendering.

---

## NON-NEGOTIABLE STARTUP SEQUENCE

1. Read complete `SKILL.md`.
2. Read complete `REFERENCE.md`.
3. Attempt to visually inspect `reference/layout-reference.jpg`.
4. If visual access succeeds, use JPG + REFERENCE.md together.
5. If visual access fails, explicitly fall back to REFERENCE.md internally; do not guess the JPG appearance.
6. Inspect the user's uploaded source photo.
7. Lock CONTENT constraints from the source.
8. Lock STYLE constraints from JPG/REFERENCE.md.
9. Generate ONLY the lower archival illustration.
10. Preserve the user's original photo pixels for the upper panel.
11. Composite the final poster.
12. Run QC against source fidelity and reference specification.

Do NOT ask the image model to generate the complete top+bottom poster in one pass.

The central rule is:

**TOP = ORIGINAL PIXELS. BOTTOM = GENERATED INTERPRETATION.**

---

## OUTPUT CONTRACT

- exactly one poster;
- strict vertical 3:4;
- upper/lower approximately 1:1;
- clean straight horizontal split;
- no collage overlaps or graphics crossing the split.

### Upper panel

Must be the actual uploaded source image.

Allowed: proportional crop only.

Forbidden: AI redraw, regeneration, mirroring, stretching, moving objects, changing architecture, adding/removing people/furniture, replacing products/materials, stylistic recoloring.

### Lower panel

Must depict the SAME scene from the SAME viewing direction and preserve source identity, but render according to `REFERENCE.md` and, when visually accessible, `reference/layout-reference.jpg`.

---

## MANDATORY WORKFLOW

### PASS A — REFERENCE LOCK

Read `REFERENCE.md` completely. If JPG visual access exists, inspect it too.

Lock:

- layout rhythm;
- illustration-to-paper ratio;
- line weight and irregularity;
- hatching density/direction;
- abstraction level;
- dark-ink mass behavior;
- paper warmth;
- one-spot-color restraint;
- print texture strength;
- typography scale/placement;
- negative-space behavior;
- overall editorial quietness.

These are STYLE LOCKS.

### PASS B — SOURCE LOCK

Analyze the user source photo and lock:

- scene type;
- camera direction and eye level;
- architecture;
- hero furniture/object;
- major furniture count and silhouettes;
- lamps, plants, artwork, shelving/audio/objects where present;
- foreground/middle/background;
- overlaps and occlusions;
- dominant lighting direction;
- one suitable muted accent color;
- factual metadata supplied by the user.

These are CONTENT LOCKS.

Never invent missing metadata.

### PASS C — GENERATE LOWER PANEL ONLY

Use CONTENT LOCKS for WHAT appears and STYLE LOCKS for HOW it is rendered.

Preserve architecture, viewpoint, furniture count/identity, object positions, foreground/background order, major silhouettes, and scene identity.

Use the detailed visual specification in `REFERENCE.md`; do not reduce it to generic adjectives such as “retro”, “vintage”, or “Riso poster”.

### PASS D — COMPOSITE

Prefer a programmatic image compositor when available.

- create strict 3:4 vertical canvas;
- place ORIGINAL source photograph in upper ~50%;
- crop proportionally, never stretch;
- place generated archival artwork in lower ~50%;
- straight clean divider;
- typography stays in lower panel;
- no cross-boundary graphics.

Compositing is mandatory because an image generator cannot be trusted to preserve exact source pixels when asked to create the whole poster.

---

## FIDELITY PRIORITY

For WHAT is depicted, source fidelity wins:

1. architecture;
2. viewpoint;
3. furniture count;
4. furniture identity;
5. object placement;
6. foreground/background order.

For HOW it is depicted, `REFERENCE.md` / visually accessible JPG wins:

1. layout hierarchy;
2. line/hatching language;
3. abstraction level;
4. paper/ink relationship;
5. limited color behavior;
6. print texture;
7. typography scale and spacing.

Never redesign the source room to resemble the reference room.

---

## REFERENCE SPECIFICATION IS MANDATORY

`REFERENCE.md` contains the detailed reproducible specification for:

- overall design character;
- poster geometry;
- lower-panel composition;
- scene fidelity;
- illustration abstraction;
- line language;
- value structure;
- color percentages/behavior;
- paper/print texture;
- typography;
- spacing/rhythm;
- hero-object handling;
- architecture handling;
- forbidden visual drift;
- canonical generation intent.

Do not skip it. Do not replace it with a short summary.

---

## TYPOGRAPHY

Typography is tiny archival metadata, never the main headline.

Use monospaced/typewriter/technical catalogue character, restrained scale, simple alignment, and generous breathing room.

Possible structure:

`No. 041`

`material / light / furniture / atmosphere`

Optional factual date/location only when known.

One short observational sentence may be used.

Language is contextual. Never invent city, country, architect, designer, brand, product model, date, or event.

---

## NEGATIVE CONSTRAINTS

Do not drift into:

- generic retro poster;
- clean flat vector;
- watercolor;
- anime/cartoon;
- glossy CGI/3D;
- photorealistic redraw;
- luxury redesign;
- unrelated Bauhaus geometry;
- scrapbook collage;
- stickers/arrows/random graphic devices;
- vivid full-color illustration;
- heavy grunge/aged paper;
- fantasy architecture;
- added decor;
- oversized advertising typography.

---

## FINAL QC

### Against source photo

- [ ] same scene identity;
- [ ] same viewing direction;
- [ ] architecture corresponds;
- [ ] major furniture count corresponds;
- [ ] hero furniture recognizable;
- [ ] major object positions correspond;
- [ ] no important invention/removal/mirroring/redesign.

### Against REFERENCE.md / accessible JPG

- [ ] lower panel belongs to the required design family;
- [ ] line density matches specification;
- [ ] hatching language matches;
- [ ] abstraction level matches;
- [ ] paper warmth matches;
- [ ] dark ink behavior matches;
- [ ] exactly one muted spot color is used selectively;
- [ ] print texture is restrained;
- [ ] typography is tiny and quiet;
- [ ] negative space remains intentional;
- [ ] result feels editorial, not template-like.

### Format

- [ ] strict vertical 3:4;
- [ ] upper/lower approximately 1:1;
- [ ] upper contains original source pixels;
- [ ] straight split;
- [ ] no cross-boundary elements;
- [ ] no fabricated metadata.

If the upper panel was AI-generated, the result FAILS and must be rebuilt with original pixels.

If the lower panel technically follows generic style words but does not satisfy the detailed `REFERENCE.md`, the result FAILS and should be regenerated.

---

## NEW-CHAT INVOCATION

When invoked from a new chat, the assistant MUST retrieve `SKILL.md` and `REFERENCE.md` before generation. It should also attempt `reference/layout-reference.jpg`, but inability to decode the JPG must NOT block correct execution: `REFERENCE.md` exists specifically as the reliable visual-spec fallback.

Recommended user invocation:

“读取并严格执行 GitHub 上 karylee996/Interior-Archive-Print 的完整 SKILL.md 和 REFERENCE.md；如果 reference/layout-reference.jpg 可以被视觉读取，也必须作为参考。不要根据仓库名称自行猜测风格。按 Skill 处理我上传的照片。”

**USER PHOTO = WHAT. REFERENCE = HOW. SKILL = PROCESS.**
