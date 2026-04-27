---
name: dark-luxury-editorial-web
description: Build or refine travel guides, 路书设计网页, editorial landing pages, and lifestyle microsites in a restrained dark luxury / Kinfolk-inspired aesthetic using React + Tailwind CSS. Use when the user asks for 高级、惊艳、克制、有呼吸感的暗黑杂志风页面，尤其是要把原始旅行攻略、行程路书、游记文本转成可交互网页、需要 Hero 与下一屏无缝过渡、优雅时间轴、地点/食物标签、低饱和 earth/forest 配色、内嵌 BGM、Pixabay 素材 sourcing / generation，或要把这套体系沉淀成 Cursor 规则 / SOP / skill 的场景。
---

# Dark Luxury Editorial Web

Use this skill to turn travel text or travel intent into a warm, restrained, benchmark-family editorial microsite.

The target feeling is:

- cinematic but quiet
- human, not system-like
- photography-led
- mobile-first
- shareable as a real destination page, not a demo shell

## Primary promise

This skill helps Codex make a route guide or memoir page that feels like the shipped Xishuangbanna / Jingshan family:

- strong Hero cover
- seamless Hero-to-second-screen continuity
- elegant itinerary structure
- restrained motion
- real imagery
- optional BGM with a real player state

## Progressive disclosure contract

This file is the entry router, not the full manual.

Default behavior:

1. read this file first
2. identify the task shape
3. load only the one or two reference files needed for that task
4. avoid bulk-loading every reference unless the task truly spans planning, writing, design, assets, and deployment at once

If the task is narrow, keep context narrow.

Examples:

- user gives only travel intent
  - read `references/intent-to-itinerary-planning.md`
  - then read `references/workflow-from-brief-to-site.md`
- user gives a finished route guide or memoir draft
  - read `references/workflow-from-brief-to-site.md`
- user says the page looks off
  - read `references/benchmark-project-family.md`
  - then `references/implementation-recipes.md`
- user says the pictures or music feel wrong
  - read `references/image-and-audio-pipeline.md`

## Non-negotiables

1. Do not overwrite a different destination project unless the user explicitly asks to replace it.
2. Treat the Hero and the next section as one continuous composition, not two slabs.
3. Blur belongs to the shared background layer, not the visible Hero image.
4. Existing benchmark-family visual rules are binding unless the user explicitly changes them.
5. Mobile is a first-class review surface, not a later cleanup pass.
6. User-facing copy must sound like a caring human travel companion, not a planner console, audit log, or system report.
7. Tags are only valid when they are concrete `place / destination` or `food`.
8. Real imagery is mandatory for a passing route-guide page; text-only dark shells, flat SVGs, muddy thumbnails, or semantically wrong images do not count.
9. A factually correct but visually flat image still fails; semantic fit and editorial beauty are both required.
10. Music UI must follow the real media element state; do not fake playback visually.
11. For 0-to-1 route planning, map validation and weather adaptation are mandatory backstage inputs, but they should not surface as stiff visible modules unless the user asks.
12. Do not invent dashboard cards, KPI blocks, validation panels, or repeated generic module shells that push the page toward AI UI.
13. If the route-loop, timeline, or vinyl player cannot reach benchmark quality, simplify or omit it instead of shipping a weak version.
14. A cold-start validation is not complete without a public deploy URL or a clearly evidenced blocker, plus browser-verified visual review.
15. Hero background image tone and Hero title color must maintain strong enough contrast to read at first glance; if the image is too close in value, fix it with image choice, overlay tuning, or text shadow before shipping.
16. Hero title must be optically centered as one composition. If the wording creates an asymmetric center, correct it with size, tracking, shell width, or simplified wording; if that still fails, recommend better wording to the user instead of forcing a broken title.

## Choose the path

### 1. User only gives travel intent

Examples:

- “从哪里去哪里，做一个几天几夜路书”
- “帮我规划一个适合家庭 / staycation / 自驾的行程”

Read:

1. `references/intent-to-itinerary-planning.md`
2. `references/workflow-from-brief-to-site.md`

Use this path when the job includes planning the trip itself before building the page.

### 2. User gives route-guide text, notes, doc, Notion, Feishu export, or partial page

Read:

1. `references/workflow-from-brief-to-site.md`

Then load additional references only as needed:

- writing tone
  - `references/editorial-writing-and-mood-mapping.md`
- visuals regressed
  - `references/benchmark-project-family.md`
  - `references/implementation-recipes.md`
- assets or music need sourcing
  - `references/image-and-audio-pipeline.md`

### 3. User is refining an existing benchmark-family site

This is usually a visual-regression or interaction-polish task.

Read:

1. `references/benchmark-project-family.md`
2. `references/implementation-recipes.md`
3. `references/failure-modes-and-qa.md`

Use this path for:

- Hero centering drift
- Hero / second-screen seam
- timeline misalignment
- player inconsistency
- too many cards / modules
- imagery that feels random or plain

### 4. User is mainly asking about images, music, or asset sourcing

Read:

1. `references/image-and-audio-pipeline.md`

This file covers:

- Pixabay-first sourcing
- Pinterest for scene discovery
- fallback order
- editorial beauty filter
- music recommendation flow
- provenance rules

### 5. User mainly needs copy shaping or memoir restoration

Read:

1. `references/editorial-writing-and-mood-mapping.md`

Use this when the page needs:

- more first-person warmth
- less AI summary language
- cleaner route-guide phrasing
- better mood-to-shot mapping

### 6. User wants reusable implementation patterns

Read:

1. `references/implementation-recipes.md`

Use this for:

- Hero layering
- title axis handling
- timeline node treatment
- route-loop presentation
- image surfaces
- audio engine behavior
- font delivery control

### 7. User wants future product evolution, not just today’s skill

Read:

1. `references/skill-to-product-evolution.md`

This is for forward planning such as `Plan -> Trip -> Memoir` productization, not for normal page delivery.

## Default operating sequence

Unless the task is unusually narrow, the safest sequence is:

1. protect project boundaries
2. determine whether this is planning, transformation, or refinement
3. load the minimum needed reference
4. normalize the content before styling
5. fix structure before effects
6. source real assets before calling the page complete
7. run mobile review before deployment
8. deploy and browser-check before final signoff

## Output expectations

### For 0-to-1 route-guide creation

Expected backstage artifacts:

- planning artifact
- research record
- real local image assets
- optional music provenance

Expected delivery state:

- built page
- public Vercel URL or a real blocker
- browser verification with visual evidence

### For refinement work

Expected delivery state:

- the regression is fixed in code
- the benchmark family is preserved
- no new module language is introduced casually

## Reference map

Read only the file you need:

- [benchmark-project-family.md](references/benchmark-project-family.md)
  Visual baseline, pass/fail sniff test, benchmark-family rules.
- [workflow-from-brief-to-site.md](references/workflow-from-brief-to-site.md)
  End-to-end build flow from raw travel material to deployed page.
- [intent-to-itinerary-planning.md](references/intent-to-itinerary-planning.md)
  0-to-1 planning logic, template selection, research stack, map and weather rules.
- [image-and-audio-pipeline.md](references/image-and-audio-pipeline.md)
  Shot list, image sourcing, beauty filter, music selection, provenance, fallback.
- [implementation-recipes.md](references/implementation-recipes.md)
  Concrete React + Tailwind patterns for the benchmark family.
- [editorial-writing-and-mood-mapping.md](references/editorial-writing-and-mood-mapping.md)
  Human-facing copy constraints and mood-to-visual translation.
- [failure-modes-and-qa.md](references/failure-modes-and-qa.md)
  Common failure patterns, regression triage, and final QA checks.
- [skill-to-product-evolution.md](references/skill-to-product-evolution.md)
  Product evolution thinking beyond the current skill.

## Preferred external helpers

These are optional helpers, not hard prerequisites.
If unavailable, keep the capability and use web fallbacks rather than blocking.

- mainland-China map primary
  - `skills.volces.com@amap-maps`
- global map supplement
  - `tivojn/google-maps-api-skill@google-maps-api`
- weather primary
  - `skills.volces.com@weather-openmeteo`
- weather fallback
  - `chandima/agent-skills@weather`

If the current environment lacks map or weather capability:

1. try installing an appropriate helper through `skills`
2. if installation fails, record that in the research artifact
3. continue with documented map / official-web / forecast fallback

## Final reminder

This skill does not define success as “a dark page with travel text”.
It defines success as:

- a benchmark-family editorial travel page
- with human warmth
- real route logic backstage
- beautiful and section-matched assets
- and a polished mobile experience

If the result still reads like a prototype, dashboard, or AI summary shell, it has not passed.
