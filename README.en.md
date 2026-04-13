[简体中文](./README.md)

# Dark Luxury Editorial Web Skill

Not for pasting travel notes onto a webpage.  
For turning travel material into a site that actually feels worth sharing.

This skill is built for the very common situation where the content is good, the taste is there, but the finished page somehow still looks flat, generic, or stitched together.  
It does not only care about copy placement. It cares about the Hero, the next screen, the images, the tags, the music, the mobile layout, and even the build size.

## What Problem Does It Solve?

Most travel pages do not fail because the content is bad.  
They fail because of things like:

- the Hero and the next section feel like two disconnected slabs
- AI can generate a page, but it often ends up as “dark background plus some text”
- tags are vague, images are semantically off, and timelines feel stiff or template-like
- the desktop version looks acceptable, but mobile immediately falls apart
- background music, asset sourcing, and font payload issues show up at the worst possible moment

This skill exists to turn those recurring problems into explicit rules before they become rework.

## When Would You Actually Use It?

### 1. You already have a route guide and want to turn it into a site

Maybe your input is:

- a Feishu doc
- a Notion page
- a Word / DOCX file
- a cleaned-up chat log

You do not just want to “publish it as a webpage.”  
You want:

- a strong cover-led first screen
- a seamless transition into the second screen
- clear daily structure without losing atmosphere
- something polished enough to send to friends without apologizing first

### 2. You only have a travel intention, not a finished itinerary

Maybe you only know:

- from where to where
- how many days
- what kind of mood you want
- roughly what budget you have

This skill can help turn that into a complete route guide first, then into a real editorial travel page.  
In other words, it can support both planning and presentation.

### 3. You have a first-person travel memoir and want to keep the original voice

Many tools flatten memoir writing into a tidy but lifeless summary.  
This skill explicitly separates route-guide mode from memoir mode, so the structure can improve without washing the author out of the page.

### 4. You already have a half-finished travel site, but it still feels off

This is exactly the kind of cleanup it is good at:

- fixing Hero / second-screen seams
- simplifying heavy or awkward timelines
- correcting visual centering and hierarchy
- forcing tags and imagery back into semantic alignment
- making the music control feel integrated instead of bolted on
- keeping font choices from silently bloating the build

## How Does It Help?

### Step 1: It identifies what kind of input you gave it

It distinguishes between:

- travel intent
- route guide
- first-person memoir

Because those should not be forced into the same page structure.

### Step 2: It structures the content before styling it

It pulls out things like:

- Hero title and subtitle
- day structure
- timeline nodes
- place / food tags
- supporting modules such as packing, transport, stay, food, and budget

The logic gets cleaned up before the polish begins.

### Step 3: It treats imagery as part of the architecture

This skill expects you to:

- define a shot list first
- source imagery early
- store the chosen assets locally
- then build the Hero and next-screen continuity around those real assets

So the page does not end up asking for good images after the layout is already locked.

### Step 4: It watches the details that usually make or break the result

It explicitly checks:

- whether the Hero-to-next-screen transition shows a seam
- whether the timeline line pierces the node
- whether tags are concrete place / food labels instead of filler
- whether music UI matches real playback state
- whether the mobile hierarchy, line-height, and center of gravity still hold
- whether Chinese font choices are quietly wrecking the build output

## Why Is It Better Than a Generic Page Generator?

Because it does not stop at “make it look premium.”  
It encodes the kinds of problems that show up again and again in real travel projects and turns them into an operational workflow.

It is a good fit if your goal sounds like this:

- I want a travel page that does not feel AI-generic
- I want consistent taste without re-debugging the Hero every time
- I want one system that can handle both itineraries and memoirs
- I want a skill that can survive a real cold-start test, not just generate instructions

## Real Outputs

These are real project outputs from the benchmark family and cold-start validation flow.

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

## What’s In This Repository?

- `dark-luxury-editorial-web-skill/`
  Full skill source

- `dark-luxury-editorial-web-skill/SKILL.md`
  Core workflow, guardrails, visual system, and QA rules

- `dark-luxury-editorial-web-skill/references/`
  Benchmarking, itinerary planning, writing guidance, implementation recipes, and media workflow references

- `dist/dark-luxury-editorial-web-skill.skill`
  Packaged installable artifact

## How Can You Use It?

The most common ways are:

1. Install the `.skill` artifact and use it directly in new travel-web projects
2. Use `SKILL.md + references/` as an editable workflow baseline
3. Use it to calibrate your own travel-web agent so it stops producing template-looking itinerary pages

## Install Artifact

- `dist/dark-luxury-editorial-web-skill.skill`

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

## Current Version

- `v1.0.0`
