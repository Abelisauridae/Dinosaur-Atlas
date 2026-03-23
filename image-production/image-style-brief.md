# Dinosaur Atlas House Style Guide

## Goal

Create a consistent 110-image painted paleoart set for the atlas:

- 107 family images
- 3 major-clade fallback images for species without family data

This guide is based on the approved reference direction: cinematic, painterly, natural-history dinosaur portraits with strong anatomy, rich texture, and dramatic but controlled environments.

## Core visual identity

- painterly realism, not flat iconography
- cinematic but still natural-history focused
- warm sunlight with atmospheric depth
- strong anatomical readability at both full size and thumbnail size
- family-defining traits should be obvious immediately
- landscapes should support the animal, not overpower it

## Composition lock

- landscape format for every image
- one featured adult animal per image
- full body visible from head to tail
- low-to-mid camera angle
- 3/4 profile or strong side-profile hero view
- animal fills roughly 60 to 75 percent of the frame
- no cropped tails, feet, horns, plates, sails, or necks
- no text, labels, frames, logos, or watermarks

## Background rules

- believable prehistoric habitat
- painterly depth with foreground, midground, and atmospheric distance
- keep the family silhouette readable against the background
- use environmental drama sparingly and intentionally
- volcanoes, storms, fire, or combat should be rare exceptions, not the default
- default mood should feel museum-quality, epic, and plausible rather than monster-movie chaotic

## Lighting rules

- warm natural light, usually morning or late-afternoon sun
- one clear primary light direction
- soft atmospheric haze in the distance
- enough rim or side light to separate the animal from the background

## Anatomy rules

- preserve recognizable family-level morphology
- avoid fantasy spikes, extra horns, monster teeth exaggeration, or oversized claws unless family-appropriate
- feathers only where appropriate for that lineage
- musculature should feel grounded and believable
- keep poses dynamic but not anatomically broken

## Consistency rules

- same aspect ratio across all images
- same rendering style across all batches
- same general contrast and color intensity
- same level of painterly finish
- same “hero portrait in habitat” framing logic

## What to avoid

- cartoon style
- toy-like surface finish
- random extra animals stealing focus
- overly dark scenes where the silhouette disappears
- excessive gore or violence
- open-mouth roaring in every image
- generic dragon-like theropod look reused across unrelated families

## Recommended export spec

- aspect ratio: 16:9
- working size: 1536 x 864 or larger
- delivery format: PNG for app use
- keep a master prompt and revision log for every image

## Production workflow

1. Use `family-image-manifest.csv` as the master checklist.
2. Generate approval rounds in small body-plan batches.
3. Lock the visual treatment after each approved batch.
4. Store metadata for every image:
   - `image_id`
   - `taxon`
   - `level`
   - `prompt`
   - `negative_prompt`
   - `model_or_artist`
   - `revision`
   - `license`
   - `approved`
