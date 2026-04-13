# Intent To Itinerary Planning

Use this reference when the user does not already have a finished route guide and instead wants Codex to plan the trip from 0 to 1.

Typical prompts:

- “从武汉去西双版纳，做一个七天六夜的路书”
- “两个人清明去襄阳，帮我规划”
- “想从上海去杭州，做一个安静一点的两天微度假网页”

## 1. Intake checklist

Always try to determine:

- origin
- destination
- trip duration
- travel dates or season
- number of travelers
- trip type
  - city walk
  - nature
  - food-first
  - family
  - couple
  - photography
  - mixed
- budget level
- transport preference
- whether the final output should skew practical or literary

If information is missing, infer conservatively and label the assumptions.

## 2. Research order

Use this order:

1. official and primary sources
2. stable current web sources
3. public UGC

Official and primary sources should be used first for:

- transport schedules
- opening hours
- ticket prices
- lodging policies
- weather or seasonal constraints

Public UGC can then refine:

- food picks
- walking rhythm
- photo spots
- queue or crowd heuristics
- what is actually worth skipping

## 3. Xiaohongshu usage rule

Treat public Xiaohongshu content as a supplemental signal source, not a source of record.

Good uses:

- finding repeated food recommendations
- identifying recent photogenic or crowded spots
- noticing practical tips that official pages omit
- spotting common itinerary mistakes

Bad uses:

- trusting one note for price or schedule
- copying one creator’s route wholesale
- treating a single viral post as representative

Best practice:

- search for multiple public note hits
- summarize recurring patterns
- cross-check practical claims against more stable sources

## 4. Minimum route-guide schema

When the user wants a full route guide, the structured output should usually include all of the following:

### 1) Itinerary overview

Include:

- total days and nights
- overall route
- daily theme summary
- who the route suits

### 2) Daily itinerary

For each day:

- day number
- one-line day title
- intro
- timed blocks

For each block:

- time
- place
- activity
- recommended food when relevant
- how to get there / distance note when relevant
- ticket / reservation note when relevant
- 1 to 2 practical tips when needed

### 3) Pre-trip preparation

Include:

- weather-aware packing
- footwear
- rain / sun / thermal needs
- medications or small utilities if relevant
- digital prep
  - booking apps
  - map apps
  - ticketing

### 4) In-trip cautions

Include:

- crowd rhythm
- weather risks
- walking intensity
- reservation timing
- cash / mobile payment edge cases
- local etiquette or scenic-area constraints when relevant

### 5) Transport and lodging

Include:

- how to reach the destination from origin
- local transport strategy
- where to stay and why
- hotel selection logic
  - convenience
  - atmosphere
  - budget
  - access to morning / night scenes

### 6) Food and specialties

Include:

- what to eat on the route
- what is destination-specific
- what can be bought as take-home specialties
- rough per-item price bands where helpful

### 7) Budget

Budget should be structured by category:

- intercity transport
- local transport
- lodging
- tickets
- food and drinks
- buffer / extras
- souvenir allowance if relevant

Give a range, not a fake-precision exact number.

## 5. Output style rules

- plan for usefulness first, polish second
- compress without losing decision-making value
- keep the plan realistic by day length and transit burden
- do not overpack every day
- leave breathable gaps in at least some days

## 6. Hand-off to webpage production

Once the route guide is planned:

1. convert it into the route-guide structure used by the main skill
2. create the shot list
3. decide the music direction
4. move into the standard page workflow
