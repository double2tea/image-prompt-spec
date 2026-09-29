---
name: image-prompt-spec
description: Write still and video prompts for Nano Banana, Seedream, GPT Image, Qwen, Seedance, Kling, and Veo. Use for generation, editing, reference roles, model choice, or a shot that must stay consistent. Includes production experience from long-form AI film work. Does not cover vendor UI, credits, CLI, or Soul slots.
license: MIT
metadata:
  type: workflow
  version: "1.1"
  source: Model dialects and field rules kept. Platform controls removed.
---

# Image and video prompt spec

Reply in the user's language. Deliver the prompt in English unless the target is Qwen and the user wants Chinese typography.

This skill covers models and production experience. It does not cover a vendor's buttons, credit prices, CLI flags, catalog ids, or account features.

## Load map

Read only the file the job needs.

- Still image — `references/image.md`
- Video shot — `references/video.md`
- Which model, and how to write for it — `references/models.md`
- Edit, references, sheets — `references/edit.md`
- Consistency, iteration, acting — `references/discipline.md`
- Worked briefs — `references/examples.md`

## Hard rules

1. Name the finished object first: poster, sheet, keyframe, or shot.
2. Write what a camera can see. Material, light direction, position. No "8K masterpiece".
3. Every reference has one role. Identity, style, product, light, location, or motion. See `references/edit.md`.
4. With an identity reference attached, do not restate the face. Without one, paste the same descriptor every shot, word for word.
5. On-image or spoken text goes in quotes. Duration and aspect ratio are job settings, not prompt magic.
6. One change per edit. Mask the change back onto the untouched original. Do not run an identity base through a full generation twice.
7. Same flaw twice means rewrite. Do not reroll the same sentence. Stop ladder is in `references/discipline.md`.
8. Keep the skeleton. Change density per model. See `references/models.md`.
9. There is no single best model. Route by asset class, then compare two if the job is close.

## Delivery

1. The brief, ready to paste.
2. The model and the one dialect adjustment.
3. The reference role list, or a note that a role is missing.
4. If this is a scene, the locked geography block, unchanged from the previous shot.
