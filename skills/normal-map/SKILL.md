---
name: normal-map
description: Create and validate normal maps for pixel Sprite atlases without damaging identity colors or frame alignment.
---

# Normal Map

Read docs/04_ART_BIBLE.md and the relevant Sprite packet before work.

## Requirements

- Match diffuse width, height, atlas layout and transparent regions exactly.
- Record coordinate convention; for Godot use the convention selected by the current
  renderer prototype rather than guessing.
- Preserve crisp alpha boundaries and use nearest filtering for pixel content.
- Derive normals from intentional form, not only a generic edge filter.
- Keep faces and identity colors recognizable under the approved lighting tests.
- Explicit Unlit content may omit a normal only when the packet records that decision.

## Review

Inspect neutral, warm and cool lights; multiple Sprite directions; atlas seams;
transparent edges; and the same scene with lighting disabled. A size match is only a
mechanical check, not visual acceptance.
