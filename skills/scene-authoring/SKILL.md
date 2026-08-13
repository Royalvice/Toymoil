---
name: scene-authoring
description: Build Toymoil scenes whose persistent world is visible and editable in Godot while runtime-spawned templates remain independently previewable.
---

# Scene Authoring

Read docs/05_SCENE_AUTHORING.md before modifying a main room or reusable template.

## Persistent scene content

Save the room structure, primary props, camera, lights, persistent actor, collision,
navigation and markers into the scene or referenced editable resources. Opening the
main scene must show the intended persistent composition without running the game.

Editor tools may generate content, but they must save deterministic editable outputs.
Do not use _ready() to construct the whole visible world from an empty root.

## Dynamic content

Enemies in waves, projectiles, drops and transient VFX may spawn at runtime. Each kind
needs an independently openable template scene or resource and a simple preview path.
Runtime code selects and drives templates; it does not hide their visual structure in
constants.

## Verification

Save, close and reopen the scene; verify the persistent composition, node ownership,
collision, navigation and preview templates. Then run the scene and confirm that no
duplicate persistent world is spawned.
