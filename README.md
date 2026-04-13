# Dark Luxury Editorial Web Skill

This repository packages the current `dark-luxury-editorial-web` skill for reuse and GitHub distribution.

## Contents

- `dark-luxury-editorial-web-skill/`
  The full skill source, including `SKILL.md`, `agents/`, and `references/`.
- `dist/dark-luxury-editorial-web-skill.skill`
  Packaged installable artifact generated from the current skill source.

## Skill Focus

This skill is for building and refining dark luxury editorial travel microsites, route-guide pages, and first-person travel memoir web experiences with:

- Hero and second-screen seamless image continuity
- Refined place and food tagging rules
- Mobile-first editorial layout and motion guidance
- Pixabay-first media sourcing with explicit fallback rules
- Audio workflow guidance
- Cold-start route-guide generation and QA rules

## Packaging

The `.skill` artifact in `dist/` was generated from the exported source with:

```bash
python3 /Users/yusijua/Desktop/skills/source/skill-creator/scripts/package_skill.py skill-github-export/dark-luxury-editorial-web-skill skill-github-export/dist
```
