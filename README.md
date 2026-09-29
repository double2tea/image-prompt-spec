# image-prompt-spec

Still and video prompts for Banana, Seedream, GPT Image, Qwen, Seedance, Kling, Veo, Hailuo, and Wan.

v1.1 puts back model dialects and production experience. v1.0 had cut those with the platform layer.

## Kept

- Asset-class routing and per-model density
- Reference roles, sheets, mask-back edits
- Video skeleton: geography lock, counts, acting, voice, style prefix
- Stop rules and the open disagreements

## Removed

Vendor UI, credits, CLI flags, catalog ids, Soul slots, Cinema Studio version pickers, apps, and marketing presets.

Source discipline is the Hell Grind pipeline as digested in OSideMedia/higgsfield-ai-prompt-skill (MIT), plus Google and OpenAI image guides. This repo does not ship their prompts or assets.

## Install

```bash
git clone https://github.com/double2tea/image-prompt-spec.git ~/.claude/skills/image-prompt-spec
```

## Map

| File | When |
|---|---|
| SKILL.md | trigger and hard rules |
| references/image.md | a still |
| references/video.md | a shot |
| references/models.md | which model, how dense |
| references/edit.md | an edit or a reference |
| references/discipline.md | consistency and when to stop |
| references/examples.md | a worked brief |
