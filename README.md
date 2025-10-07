# Legion Remix — Codex Pack

This pack gives you a clean loop between your local **Legion Remix** logs and **ChatGPT** for creative writing.

## What’s inside
- `characters/`, `events/`, `arcs/`: your source-of-truth world files
- `style/`: tone board and style rules
- `templates/creative_brief.md`: the export format ChatGPT will consume
- `commands/make-brief.yaml`: Codex command to compile a brief
- `briefs/`: output destination for generated briefs
- `.codex/`: optional rules and lint config for your workspace (customize freely)
- `MANIFEST.md`: quick reference of files and their purpose

## Quick start
1) Drop your character/event/arc Markdown files into the respective folders.
2) Run the Codex command `make-brief` with a scope, e.g. `all-recent` or a list of event ids.
3) Open the generated `briefs/latest_brief.md`, copy it, and paste into ChatGPT with this wrapper:

> **TASK:** Write a [scene/recap/dialogue] ~600–900 words. Keep canon facts inviolable. Match tone board. Use seed lines sparingly. End with a hook.  
> **OUTPUT:** Markdown only. No meta commentary.

## Scope examples
- `all-recent` → compiles the last few events
- `events/week-01,events/week-02` → compiles by explicit slugs
- `events/nighthold-guldan` → compile a single event

---

Tip: Keep character cards short (≤7 lines each) and keep `Canon Facts` to 5–15 bullets for best prompt efficiency.
