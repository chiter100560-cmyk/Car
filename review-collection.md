# Competitor review teardown — the 20-minute manual pass

The one job that keeps getting blocked. Nothing here needs skill, only your phone
and twenty minutes. Do it once and it becomes website copy and operating rules.

## Status

| Business | State |
|---|---|
| One Call Detailing, Pompano Beach | **Done** — 5.0 / 585, five negatives total, four with text. In `complaints.html` §00 |
| Mobile Detailers Inc, Coral Springs | **Counted, not read** — 4.9 / 34 on Google, one 1-star. Highest-value gap |
| Platinum | **Wrong name** — no exact match. Closest: *PLATINUM – Mobile Auto Detailing*, 8383 NW 57th Dr, 4.9 / 77. Confirm the listing |
| GoFilms Window Tinting, Plantation | Not reached |
| Family Mobile Window Tint, Margate | Not reached |

**What works:** the Claude desktop app on the Mac, with a connected browser. Not a
cloud session — see below.

**What broke:** Google Maps stopped responding after the first listing — the sort menu
would not apply and more reviews would not load. **Fix: one business per fresh tab, and
close the tab before starting the next.**

**Do the two tint businesses first** from here. You have never tinted a car, so their
complaints are worth more to you than another detailer's: they will be about bubbles,
creases, peeling, purple film, cure-time confusion and damaged defroster lines — the
exact things you are about to be bad at.

**No verbatim quotes.** Reviewers own their words. Paraphrase point by point, keep the
star count and date, and note which keywords appear in the original.

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
