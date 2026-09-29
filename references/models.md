# Models

Routing is by asset class, from the AI-vs-VFX production build (2026-08). Switching models mid-project is normal. Credits and UI toggles are omitted on purpose.

Skeleton for stills is `image.md`. Skeleton for shots is `video.md`. Roles are `edit.md`.

## Stills

| Job | First try | Why | How to write |
|---|---|---|---|
| Human sheet, face match, one-line fix | Nano Banana 2 | Holds the input; strongest face match in that build | Short narrative. One change. Do not rebuild the sheet |
| 4K, many references, poster text | Nano Banana Pro | Reasoning before draw; text and layout | One or two sentences plus blocks. Quote text and place it. Lens numbers are weak |
| Fantasy creature, stylized 2D, manga panels | Seedream 5.0 Pro | Line, flat color, non-human sheets | Physical surfaces, art-era anchor. Name wear and weight |
| Clothing, branded garments, UI, quoted text | GPT Image 2 / 2.5 | Clothing and layout. 2.5 adds transparent background and higher quality tiers | Format A JSON for regions; Format B prose for one scene; tie goes to A. Do not say photorealistic for faces |
| Chinese layout, named school | Qwen Image | School names and CJK type respond | Quoted Chinese, position, type role |
| Cinematic location plate | A cinema-still model, or Banana if identity must hold | GPT location stills skew yellow; Banana locations go too clean and symmetrical | 3/4 view, one light, an anchor object. Select on light, not on prettiness |
| Costume texture from scratch | OPEN | One build used GPT for wardrobe edits; another used Seedream 5 Pro for costume texture. Compare 2-3 | Do not declare a winner from one seed |

Banana: physical light and place, not artist-name soup.
Seedream: materials. Weak when the same sentence also demands exact Latin/CJK layout.
GPT: quote exact strings. Film-photo language for skin.
Qwen: medium name allowed. Still assign reference roles.

## Video

| Job | First try | How to write |
|---|---|---|
| Multi-reference, edit, extend | Seedance 2.0 / 2.5 | Role each reference. Motion and camera if a start frame is attached. Identity text stays identical and never contradicts the image |
| Physics, dance, sport | Hailuo 2.3 | Weight, contact, inertia. Not mood adjectives |
| Vehicle chase, native audio | Veo 3.1 | One action. Quote dialogue once |
| Start-frame animation, budget cinematic | Kling 3.0 / 3.0 Turbo | Start image carries frame one. Prompt carries motion only |
| Stylized, painterly | Wan 2.6 / 2.7 | Name the medium. Do not mix a photoreal identity lock in the same sentence |
| Talking head from a still | Seedance 1.5 Pro class | Locked voice line plus the still. Do not redesign the face |

Sora 2 is retired at the API (2026-09-24). Do not recommend it.

## What a prompt cannot fix

The same reference and the same sentence still diverge. Each model was trained on a different prior and reads a reference as features, not pixels. Lock style in a style-only image. Do not ask the text to cancel the prior.
