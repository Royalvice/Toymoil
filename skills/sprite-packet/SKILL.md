---
name: sprite-packet
description: Define and review the reusable action, direction, timing, layer, and anchor information needed by a Toymoil Sprite actor.
---

# Sprite Packet

Read docs/04_ART_BIBLE.md and docs/05_SCENE_AUTHORING.md.

## Packet questions

- Which actions exist and what gameplay state requests each action?
- Which directions are authored, mirrored or intentionally shared?
- What is each frame duration, loop rule and transition rule?
- Where are feet, body center, shadow, hand, grip, muzzle and hit anchors?
- Which layers render behind or in front of the body for each direction?
- Is the Sprite lit, unlit, or mixed, and what paired data does it require?
- What world scale and screen-size assumptions remain provisional?

Do not name a future Godot Resource class until a real implementation needs one.
Keep collision and gameplay rules outside visible-alpha metadata.

## Acceptance

Preview every action and direction, including transitions and mirrors. Check feet and
weapon anchors for drift, hand-layer swaps, alpha seams and animation continuity.
