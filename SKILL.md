---
name: Interior-Archive-Print
description: Strict two-pass workflow for turning one interior photograph into a 3:4 vertical split poster: exact original photo on top, archival linocut/Risograph reconstruction below.
---

# Interior-Archive-Print

## READ THIS FIRST — NON-NEGOTIABLE EXECUTION RULES

This is NOT a loose style prompt.

When this Skill is invoked, the assistant MUST follow this exact workflow in order:

1. Read this entire SKILL.md before generating anything.
2. Inspect the uploaded source photo carefully.
3. NEVER ask the image model to recreate the final full poster in one pass.
4. Generate ONLY the lower archival illustration from the uploaded source photo.
5. Preserve the original uploaded photograph as real pixels for the upper half.
6. Assemble the final 3:4 poster by compositing the original photo on top and the generated illustration on the bottom.
7. Run the final QC checklist before returning the result.

If the assistant instead generates one complete image containing both the “photo” and the “illustration”, the result is considered WRONG because the upper photo may be reinterpreted, distorted, recolored, or redesigned.

The most important principle of this Skill is:

**TOP = ORIGINAL PIXELS. BOTTOM = GENERATED INTERPRETATION.**

---

## OUTPUT CONTRACT

Final output:

- exactly one poster;
- strict vertical 3:4 aspect ratio;
- upper half ≈ 50%;
- lower half ≈ 50%;
- clear horizontal split;
- no collage, no multi-photo layout, no decorative overlays crossing the split.

### Upper half

The upper half must be the actual uploaded source image, not an AI redraw.

Allowed:

- proportional crop to fit the poster;
- minor global tonal normalization only when necessary.

Forbidden:

- regenerating the room;
- moving furniture;
- changing architecture;
- adding/removing people or objects;
- mirroring;
- repainting surfaces;
- changing product design;
- replacing lighting;
- changing colors for style consistency.

### Lower half

The lower half must depict the SAME photographed space from the SAME viewpoint.

It is a stylized reconstruction, not a redesigned interior.

Preserve:

- camera direction;
- framing logic;
- major furniture count;
- furniture silhouettes;
- architectural openings;
- object positions;
- foreground / middle / background relationships;
- important occlusions;
- dominant lighting direction;
- recognizable hero objects.

---

## MANDATORY TWO-PASS WORKFLOW

### PASS A — ANALYZE AND LOCK

Before generating the lower illustration, identify:

- room type;
- camera angle and approximate eye level;
- dominant architectural lines;
- hero furniture / hero object;
- all major furniture pieces;
- plants;
- lamps;
- artwork;
- shelves / audio equipment / objects when present;
- foreground, middle ground, background;
- major overlaps;
- dominant source colors;
- ONE accent color to retain in the print;
- any factual metadata supplied by the user.

Do not invent missing factual metadata.

### PASS B — GENERATE LOWER PANEL ONLY

Use the uploaded photo as the visual reference.

Generate a lower-panel artwork with the following visual language:

**1970s–1980s interior design archive / architecture journal / independent furniture catalogue / linocut + wood engraving + screen print + Risograph.**

Base look:

- warm ivory / cream uncoated paper;
- deep brown-black ink linework;
- one muted spot color sampled from the original image;
- hand-drawn architectural line quality;
- linocut and woodcut hatching;
- cross-hatching in shadows;
- sparse halftone;
- slight ink loss;
- subtle registration imperfection;
- tactile paper grain;
- restrained hand-pulled print texture;
- premium editorial design, not distressed grunge.

The illustration must remain structurally close to the source image.

### PASS C — COMPOSITE

After the lower image is generated:

- create a 3:4 vertical canvas;
- place the ORIGINAL uploaded photo in the upper 50%;
- crop proportionally, never stretch;
- place the generated archival illustration in the lower 50%;
- preserve a clean straight horizontal boundary;
- do not let any lower-panel element overlap the upper photo;
- keep the typography entirely inside the lower panel.

If a programmatic image compositor is available, use it. This is preferred over asking the image model to generate the whole poster.

---

## LOWER-PANEL STYLE LOCK

The visual target is not merely “retro”. It should look like a page from a carefully art-directed design archive.

### Linework

Use:

- rough black/brown ink outlines;
- varied line weight;
- woodcut-style parallel hatching;
- cross-hatching for depth;
- broken print edges;
- slightly imperfect hand-made marks.

Avoid:

- clean vector outlines;
- smooth CGI contours;
- airbrushed digital shading;
- watercolor washes;
- anime/cartoon rendering.

### Color

Use a limited palette:

1. warm cream paper;
2. deep brown-black ink;
3. ONE main accent color from the source photo.

Examples:

- dominant greenery → olive / moss green;
- red shelving/art → brick red / oxblood;
- caramel leather/timber → tobacco / burnt orange;
- strong blue object → muted slate / navy blue.

Do not recreate the full photographic palette in the illustration.

### Paper and print texture

Use restrained physical-print character:

- uncoated cream paper;
- subtle grain;
- tiny print noise;
- sparse uneven ink density;
- mild Risograph misregistration;
- occasional dry-ink gaps.

Do not make the page look dirty, damaged, or artificially ancient.

---

## FIDELITY PRIORITY

When style conflicts with fidelity, fidelity wins.

Priority order:

1. architecture;
2. viewpoint;
3. furniture count;
4. furniture identity;
5. object placement;
6. foreground/background order;
7. style;
8. texture.

Never improve the room by redesigning it.

Do not:

- substitute a different sofa/chair/table;
- add decorative plants;
- remove clutter simply because it is inconvenient;
- create a more luxurious version of the space;
- change window or doorway dimensions;
- simplify the room until its identity is lost.

Small clutter may be grouped graphically, but major anchor objects must remain recognizable.

---

## TYPOGRAPHY SYSTEM

Typography must stay quiet and archival.

Preferred character:

- monospaced;
- typewriter;
- old catalogue index;
- technical archive label.

Recommended small text block:

`No. 041`

`retro corner / warm light / objects and posters`

`20XX`

`旧物与光，一角的温度刚刚好。`

The actual wording MUST adapt to the source image.

Rules:

- small type only;
- lower-left or another quiet lower-panel area;
- generous negative space around text;
- no oversized headline unless user requests it;
- no fake branding;
- no invented architect/designer/location/date.

### Language

Do NOT force Korean, Japanese, Chinese, or English.

Language is contextual.

If the location is unknown, use neutral descriptive copy instead of inventing a place.

---

## CANONICAL LOWER-PANEL GENERATION INSTRUCTION

When generating the lower panel, the assistant should internally use an instruction equivalent to:

“Using the uploaded interior photograph as the sole visual reference, reconstruct the exact same room from the same camera viewpoint as a premium 1970s–1980s interior-design archival print. Preserve the major architecture, furniture identity, furniture count, object positions, foreground/background relationships, and recognizable silhouettes. Render on warm ivory uncoated paper with deep brown-black linocut/woodcut ink lines, hand-drawn architectural hatching, cross-hatching, sparse halftone, subtle screen-print/Risograph texture, and only one muted accent color sampled from the original scene. Keep the composition faithful rather than redesigning the room. Leave controlled negative space for small typewriter-style archival metadata. No photorealism, no 3D rendering, no watercolor, no clean vector style, no anime, no furniture redesign, no extra decor, no invented architecture, no vivid multicolor palette.”

This is the visual anchor. Do not dilute it with unrelated style adjectives.

---

## ADAPTIVE RULES

### Plant-heavy rooms

Preserve the silhouette and approximate placement of the major plants. Simplify leaves into grouped engraved shapes. Accent color may be muted olive/moss green.

### Furniture-focused rooms

Preserve upholstery geometry, legs/base, cushion segmentation, arm shape, and relationship to surrounding pieces.

### Object-heavy / retro rooms

Preserve key recognizable objects such as record players, speakers, lamps, clocks, radios, globes, books, framed art, and distinctive shelving. Simplify only tiny secondary clutter.

### Minimalist architecture

Emphasize structural lines, openings, ceiling/floor geometry, furniture proportion, and negative space. Do not add texture everywhere.

---

## NEGATIVE CONSTRAINTS

The lower panel must NOT become:

- generic retro poster;
- flat vector art;
- watercolor illustration;
- cartoon;
- anime;
- realistic 3D render;
- glossy CGI;
- luxury interior redesign;
- scrapbook collage;
- Bauhaus geometric poster unless specifically requested;
- random graphic shapes;
- decorative sticker layout;
- over-distressed vintage paper;
- full-color photo tracing;
- arbitrary fantasy architecture.

---

## FINAL QC — MUST CHECK BEFORE OUTPUT

A result fails this Skill if any critical item below is wrong.

### Format

- [ ] final image is vertical 3:4;
- [ ] top and bottom are approximately 1:1;
- [ ] split is straight and clean.

### Upper panel

- [ ] upper image uses the original uploaded photograph pixels;
- [ ] no AI-redrawn upper room;
- [ ] no mirror/stretch/distortion;
- [ ] no added/removed furniture or people.

### Lower panel

- [ ] clearly depicts the same room;
- [ ] same viewing direction;
- [ ] major furniture positions correspond to source;
- [ ] architecture remains recognizable;
- [ ] no arbitrary redesign;
- [ ] palette is cream + dark ink + one principal accent;
- [ ] texture feels like linocut/woodcut/screenprint/Risograph;
- [ ] negative space remains controlled.

### Text

- [ ] small archival/typewriter typography;
- [ ] wording relates to the scene;
- [ ] no fabricated location/date/designer information.

If the top panel was regenerated by AI instead of using the original image, STOP and rebuild the poster with the original photo before returning it.

---

## INVOCATION BEHAVIOR IN A NEW CHAT

When the user says something like:

“安装 GitHub 上 karylee996 的 Interior-Archive-Print，并按这个 Skill 生成这张照片。”

The assistant should NOT immediately generate.

It should first retrieve and read the full `SKILL.md`, then silently apply the mandatory workflow above.

Do not rely on the repository name alone.
Do not summarize the Skill and then improvise.
Do not use a generic “retro interior poster” prompt.
Do not skip the compositing stage.

The reproducibility of this Skill depends on following the execution workflow, not merely matching the aesthetic keywords.
