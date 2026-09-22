# Competitor review teardown — the 20-minute manual pass

The one job that keeps getting blocked. Nothing here needs skill, only your phone
and twenty minutes. Do it once and it becomes website copy and operating rules.

## Why a cloud session can't do it

Tested 22 Sep 2026 from the Claude cloud session, with a real headless browser
(it works now — it didn't in the August session):

| Source | Result |
|---|---|
| Google Maps | Loads the shell, then Google returns **403 on its own JS bundle** — no results render |
| Google Search | **"Our systems have detected unusual traffic from your computer network"** — CAPTCHA |
| Yelp | **HTTP 403** |
| DuckDuckGo | CAPTCHA ("select all squares containing a duck") |
| Bing | Returns an empty results shell |
| Birdeye | Google reviews sit behind a JS tab; only old Facebook reviews are exposed |

These are bot protections keyed to the datacenter IP, not a bug and not something
to defeat. **A logged-in human browser on a home connection walks straight through
all of them.** That is you, on your phone, in ten minutes.

## The procedure

For each competitor:

1. Google Maps → search the business → open it
2. Tap the **review count** (not the star rating)
3. **Sort → Lowest rating**
4. Read the 1-, 2- and 3-star reviews. Ignore the 4s and 5s entirely
5. For anything that names a concrete failure, copy the review text

Then use the **Search reviews** box inside the same panel for these words, because
sorting alone misses complaints buried in otherwise-positive reviews:

> late · didn't show · no show · cancel · reschedul · refund · scratch · damage ·
> swirl · missed · spots · streak · overcharge · quote · rude · waiting · bubble ·
> peel · purple · redo

## The five businesses

1. **One Call Detailing** — Pompano Beach (~571 reviews, the benchmark)
2. **Mobile Detailers Inc** — Coral Springs (detail + tint + ceramic; the exact concept, on your street)
3. **Platinum Auto Detailing** — Coral Springs / Parkland (70+ five-star)
4. **GoFilms Window Tinting** — Plantation (~351 reviews)
5. **Family Mobile Window Tint** — Margate (closest tint competitor)

## Paste this back in

One block per review. Copy the words exactly — do not summarise, the exact phrasing
is what becomes website copy.

```
BUSINESS: One Call Detailing
STARS: 2
DATE: (month/year shown)
TEXT: "..."
---
BUSINESS:
STARS:
DATE:
TEXT: "..."
---
```

Fifteen to thirty of these across the five businesses is plenty. Paste them into a
session and the next step is mechanical: rank the themes that repeat, turn the top
ones into operating rules, and write the website copy that sells against each.

## What you already have without it

`complaints.html` covers the industry-wide complaint patterns — eight ranked
complaints, the rule that prevents each, a booking script, and website copy. That is
most of the value. The local pass adds the part that matters commercially: **anything
your five competitors get complained about that is NOT on the industry list is a gap
in your market**, and the gap is where the money is.
