# Video shots

A video model has no memory between generations. Geography and identity are pasted again, unchanged.

## Skeleton

```text
SCENE: EXACT <N> CHARACTERS — NO DUPLICATES: <names>.
GEO: <floor plan only. landmarks, frame-left, frame-right, camera side, the line it never crosses. no people, no action>
WHO: <this shot only: who stands where, in metres from a landmark, where they look>
ACTION: <one verb. charge, burst, aftermath if it is a hit>
CAMERA: <one move, or locked>
ACTING: <want, hide, body rhythm, habit, what changes>
AUDIO: "<line>" once. Voice: <register, tempo, accent, manner>
STYLE: <the project style prefix, pasted word for word>
REFS:
  @name — IDENTITY. Do not copy wardrobe from this image.
  @loc — LOCATION. Space and texture only. Do not inherit angle or grade.
```

Duration and aspect ratio are job settings. Writing "12s" or "8K" in the prose does not set them.

## Rules that came from failed shots

- First second of a scene is a populated wide with no scripted action, so positions stick. Life (breath, eyes) is allowed. A shot whose job is an event may open mid-action instead.
- After every cut, restate who stands where. Sides are frame-left and frame-right, not "left of the character".
- Count objects. "Exactly one lamp." Lead with the count.
- Start-frame job: the image is frame one. Prompt is motion and camera only.
- No reference: the descriptor is pasted word for word every shot.
- With a reference: identity text must not contradict the image. Whether to also paste the full descriptor is OPEN; never let the two disagree.
- Location reference gets an explicit ban on inheriting composition and grade.
- Dialogue: lock voice in pre-production. Register, tempo, accent, manner. Paste it whenever they speak.
- Style prefix is identical on every shot. Do not restyle per shot.

Action arc when there is a hit: plant, burst, aftermath. Do not write the result as an adjective.
