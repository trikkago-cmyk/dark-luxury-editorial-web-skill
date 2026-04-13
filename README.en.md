[简体中文](./README.md)

# Dark Luxury Editorial Web Skill

Turn raw travel text into a cinematic editorial microsite.

If your current “travel guide” is a pile of notes, a few screenshots, and a heroic amount of taste held together by sheer willpower, this skill is here to help.  
It is built for dark editorial travel pages that should feel restrained, immersive, photography-led, and genuinely worth sharing.

## What This Skill Does

This skill turns:

- route-guide drafts
- multi-day itineraries
- first-person travel notes
- loose destination ideas

into:

- travel landing pages
- interactive route-guide microsites
- first-person travel memoir websites
- mobile-first dark luxury travel experiences

Its job is not “put some words on a webpage.”  
Its job is to make the webpage feel like a place.

## Why It’s Useful

Not “just another dark page with some text on it.”  
This skill is opinionated exactly where travel pages usually go wrong:

- Hero and second-screen continuity
- the same cover image reused as the blurred world beneath the page
- place / food tags with real semantic constraints
- route-guide vs memoir content structuring
- mobile optical centering instead of desktop leftovers
- media sourcing with fallback rules instead of wishful thinking
- audio workflow guidance when the page needs BGM
- font payload control so the build does not secretly become a truck full of CJK font files

In short:  
it helps you stop shipping “text on a dark background” and start shipping travel pages that actually feel like somewhere.

## Real Outputs

These are real project outputs used as part of the benchmark family and cold-start validation workflow.

<table>
  <tr>
    <td align="center">
      <a href="https://dark-luxury-travel-itinerary.vercel.app">
        <img src="./assets/screenshots/xishuangbanna-hero-mobile.png" alt="Xishuangbanna route guide mobile screenshot" width="220" />
      </a>
      <br />
      <strong>Xishuangbanna Route Guide</strong>
      <br />
      Fuxian Lake · Xishuangbanna itinerary
    </td>
    <td align="center">
      <a href="https://wuhan-jingshan-travel-guide.vercel.app">
        <img src="./assets/screenshots/jingshan-route-mobile.png" alt="Jingshan route guide mobile screenshot" width="220" />
      </a>
      <br />
      <strong>Jingshan Route Guide</strong>
      <br />
      Wuhan · Jingshan itinerary
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://youji.travel-itinerary-jingshan.online">
        <img src="./assets/screenshots/jingshan-memoir-mobile.png" alt="Jingshan memoir mobile screenshot" width="220" />
      </a>
      <br />
      <strong>Jingshan Memoir</strong>
      <br />
      Four-day memoir site
    </td>
    <td align="center">
      <a href="https://skill-solid-coldstart-routeguide-ag.vercel.app">
        <img src="./assets/screenshots/coldstart-hangzhou-mobile.png" alt="Cold-start Hangzhou route guide mobile screenshot" width="220" />
      </a>
      <br />
      <strong>Cold-start Validation</strong>
      <br />
      Hangzhou two-day route-guide test
    </td>
  </tr>
</table>

## What’s In This Repository

- `dark-luxury-editorial-web-skill/`
  Full skill source.

- `dark-luxury-editorial-web-skill/SKILL.md`
  Core workflow, guardrails, visual system, and QA rules.

- `dark-luxury-editorial-web-skill/references/`
  Supporting references for benchmarking, itinerary planning, writing tone, implementation recipes, and media sourcing.

- `dist/dark-luxury-editorial-web-skill.skill`
  Packaged installable artifact.

## Key Capabilities

- Hero and next-screen transition rules
- route-guide and memoir structuring
- cold-start itinerary generation flow
- place / food tag semantics
- media sourcing with fallback chain
- audio direction and playback UX guidance
- font payload control for Vite travel projects

## Benchmark Family

This skill is calibrated against these live projects:

- Xishuangbanna route guide: `https://dark-luxury-travel-itinerary.vercel.app`
- Jingshan route guide: `https://wuhan-jingshan-travel-guide.vercel.app`
- Jingshan memoir: `https://youji.travel-itinerary-jingshan.online`

That means the goal is not “generically pretty.”  
The goal is to belong to the same design family: photography-led, deep green-black atmosphere, seamless Hero continuity, and restrained but intentional detail.

## Install Artifact

The packaged installable artifact lives here:

- `dist/dark-luxury-editorial-web-skill.skill`

If you only want to install the skill and skip the source layout, this is the file you want.

## Repository Structure

```text
.
├── assets/
│   └── screenshots/
├── dark-luxury-editorial-web-skill/
│   ├── SKILL.md
│   ├── agents/
│   └── references/
└── dist/
    └── dark-luxury-editorial-web-skill.skill
```

## Version

Current public release:

- `v1.0.0`
