# Failure Modes And QA

Use this reference when:

- a new page feels visually “off” even though the structure is roughly there
- a cold-start validation needs a hard pass / fail check
- an existing benchmark-family site has regressed
- you need to diagnose why the page still feels like AI UI

## Quick map

- Hero regressions
  - `Hero mistakes`
- typography and axis issues
  - `Typography mistakes`
- timeline / route-loop issues
  - `Timeline mistakes`
  - `Route-loop mistakes`
- tone and content drift
  - `Content mistakes`
- player and soundtrack issues
  - `Music mistakes`
- final triage
  - `Debug checklist`

## 1. Cold-start fail-fast rule

One serious benchmark-family miss is enough to fail the run.

Examples:

- broken Hero / next-screen continuity
- mobile Hero title breaking awkwardly
- timeline line piercing nodes
- player state drifting from the real audio element
- boxy module-heavy layout
- visible system language in the rendered page
- flat, random, or low-quality imagery

Do not “average out” a visually failed run just because the planning work backstage was strong.

## 2. Hero mistakes

Do not:

- blur the visible Hero image
- stack multiple transition strips to hide a seam
- insert an opaque slab below the Hero and call it a transition
- let the first content section crash directly into the cover
- center each Hero line separately instead of aligning one optical stack
- let the Hero cluster sit too low on mobile
- accept a cover where text readability is poor but can supposedly be fixed later

If the Hero feels wrong, inspect in this order:

1. background layer structure
2. clear Hero cover mask fade
3. shared width shell for overline, title, subtitle
4. title scale and line breaks on mobile
5. text shadow strength
6. breathing room before the second screen starts

## 3. Typography mistakes

Do not:

- let Hero text get too thin over photography
- leave supporting labels so small or light that they disappear
- allow desktop day titles to wrap casually into weak two-line headings
- use raw system labels such as `validation`, `route topology`, or `confidence` in visible copy
- let English subtitle tracking grow so wide that it destabilizes the Chinese Hero

Typography usually fails for one of two reasons:

1. the designer shrank text instead of simplifying wording
2. the axis between overline, title, and subtitle was not treated as one composition

Fix wording and shell alignment before chasing micro-spacing.

## 4. Timeline mistakes

Do not:

- let the line pierce the node
- use oversized time labels
- wrap each event in a bulky dark card
- add thick black rings around the node
- let time, node, and heading drift off the same visual baseline
- turn a floating editorial rhythm into a spreadsheet-like schedule block

The safest quality bar:

- small, restrained time
- node feels independent
- line exists only between nodes
- hover is subtle
- mobile collapses cleanly without preserving desktop rigidity

If the timeline still looks clumsy, simplify it.

## 5. Route-loop mistakes

Do not:

- show the route-loop only to prove “maps were used”
- let labels overlap or read like debugger metadata
- hide route direction so the viewer cannot tell where the trip starts or ends
- draw lines through nodes in a cheap way
- use a route diagram that visually dominates the page
- keep the module if overview prose already explains the route cleanly

Signs the route-loop should be removed or collapsed:

- it needs too much explanation text to make sense
- it introduces a new component language not used elsewhere
- it feels like a planning dashboard, not editorial guidance
- its geometry is less elegant than a short prose explanation

## 6. Content mistakes

Do not:

- add AI-ish prefatory framing the user did not ask for
- replace first-person memoir voice with generic summary prose
- expose research, confidence, validation, or provider names in visible page sections
- invent abstract tags
- omit food / specialties when the trip clearly has a food dimension
- separate support sections into too many equal-weight modules when one calmer spread would read better

The visible page should feel like it is speaking to a traveler, not documenting an internal workflow.

## 7. Music mistakes

Do not:

- let the UI imply playback when the media element is blocked or paused
- make the vinyl player oversized on mobile
- redesign the benchmark-family player into a new capsule or toolbar without explicit user direction
- let the tonearm and disc state drift out of sync
- silently reuse an old project track in a supposed cold-start validation

If autoplay is wanted:

- try it
- never trust it
- keep click-to-play fallback
- confirm the player state follows real events

## 8. Asset mistakes

Do not:

- settle for a photo just because it is geographically correct
- use watermark-heavy, archival, flat, or visibly dated imagery as final spread art
- use the same weak frontal architecture shot for both a day anchor and a support spread
- keep a low-resolution preview because the shot list is already done

The recurring trap is:

- `correct but plain`

That still fails.

## 9. Process mistakes

Do not:

- create a parallel replacement skill when the user asked to refine the current one
- stop at markdown artifacts without a public webpage when the task is cold-start validation
- rely on desktop-only review
- accept “more modules” as the solution to information clarity
- leave the export package stale after changing the local skill

## 10. Debug checklist

When a page still feels off, inspect in this order:

1. Is the visible Hero image accidentally blurred?
2. Is there a visible seam caused by an extra background or opaque slab?
3. Is the Hero stack mis-centered because the overline, title, and subtitle do not share one shell?
4. Is the Hero too low or too weak on mobile?
5. Are tags semantically wrong or visually noisy?
6. Does the timeline line pierce the node?
7. Are day images mismatched to the text?
8. Does the route-loop actually clarify the route, or is it decorative noise?
9. Does the player UI follow real playback state?
10. Is the fixed player covering too much on mobile?
11. Are there too many repeated dark boxes or panels?
12. Would a human confuse this page with the shipped benchmark family?
13. Do desktop and mobile screenshots both pass?
14. Could two or three support modules be collapsed into one calmer editorial spread?

## 11. Pass rule

A page passes only when:

- the benchmark-family structure holds
- the tone feels human
- the imagery feels intentional
- the motion stays restrained
- the player behaves truthfully
- desktop and mobile both feel like finished work

If the page still reads like a prototype, it is not done.
