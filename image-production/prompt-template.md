# Dinosaur Atlas Prompt Template

Use this as the master template for any image model or illustrator brief.

## Master prompt

```text
Create a painterly natural-history paleoart illustration of [TAXON], a [LEVEL] dinosaur group from the Dinosaur Atlas project. Show one featured adult animal in a full-body hero composition, landscape format, with the entire head, torso, limbs, and tail visible. Use a low-to-mid camera angle and a strong 3/4 profile or side profile. Emphasize the family-defining anatomy: [KEY_TRAITS]. The animal should read instantly at thumbnail size.

Visual style: cinematic painterly realism, museum-quality paleoart, rich natural textures, believable musculature, controlled atmospheric perspective, warm natural light, dramatic but plausible prehistoric environment, detailed but not chaotic background, no fantasy exaggeration.

Environment: [HABITAT]. Lighting: [LIGHTING]. Color direction: [PALETTE]. Mood: epic, grounded, scientifically inspired, elegant, and consistent with a premium dinosaur atlas.

Important constraints: one main animal only, no text, no frame, no watermark, no cropped body parts, no modern objects, no excessive gore, no cartoon styling, no generic monster look, no overdesigned fantasy spikes unless anatomically appropriate.
```

## Negative prompt

```text
cartoon, anime, toy, low detail, blurry anatomy, bad limbs, cropped tail, cropped head, cut off feet, extra horns, fantasy dragon, monster design, random fire everywhere, oversaturated neon color, modern plants, humans, text, logo, watermark, collage, multi-panel layout, scientific inaccuracy, malformed claws, duplicate limbs
```

## Per-image fill-ins

- `TAXON`: family or major clade name
- `LEVEL`: `family` or `major clade`
- `KEY_TRAITS`: 3 to 6 anatomical features that define the taxon
- `HABITAT`: broad habitat cue only, not a distracting story scene
- `LIGHTING`: usually warm morning or late-afternoon directional light
- `PALETTE`: earthy, natural, and lineage-appropriate

## House defaults

- one hero animal
- full body visible
- 16:9 composition
- warm atmospheric landscape
- painterly natural-history realism
- readable silhouette first, texture second
