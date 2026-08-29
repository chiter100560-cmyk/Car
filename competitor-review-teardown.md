# Competitor review teardown — BLOCKED, no data collected

**Status: not done. Zero reviews were collected.** This file exists so the
attempt is not silently repeated. It contains no review text, no complaint
themes, no website copy and no operating rules, because none could be
sourced. Anything below the line is method, not findings.

Attempted 2026-08-29.

## Targets

| # | Business | City | Sources wanted |
|---|---|---|---|
| 1 | One Call Detailing | Pompano Beach FL | Google Maps, Yelp |
| 2 | Mobile Detailers Inc | Coral Springs FL | Google Maps, Yelp |
| 3 | Platinum Auto Detailing | Coral Springs FL | Google Maps, Yelp |
| 4 | GoFilms Window Tinting | Plantation FL | Google Maps, Yelp |
| 5 | Family Mobile Window Tint | Margate FL | Google Maps, Yelp |

Wanted: every 1-, 2- and 3-star review, verbatim, with a source URL.

## What blocked it

The session's egress proxy enforces a **GitHub-only allowlist**. It is not
set to full network access, whatever the environment settings screen says.

Direct requests (`curl`) fail at the tunnel:

```
$ curl https://www.google.com
curl: (56) CONNECT tunnel failed, response 403

$ curl -sS "$HTTPS_PROXY/__agentproxy/status"
"recentRelayFailures": [
  { "kind": "connect_rejected",
    "detail": "gateway answered 403 to CONNECT (policy denial or upstream failure)",
    "host": "www.google.com:443" },
  { ... "host": "www.yelp.com:443" },
  { ... "host": "www.bing.com:443" }
]
```

Page fetches through the harness fail the same way. Every domain tried
returned `EGRESS_BLOCKED`:

| Domain | Result |
|---|---|
| `www.yelp.com` | EGRESS_BLOCKED |
| `www.google.com` (Maps) | EGRESS_BLOCKED |
| `reviews.birdeye.com` | EGRESS_BLOCKED |
| `www.bbb.org` | EGRESS_BLOCKED |
| `washindex.com` | EGRESS_BLOCKED |
| `local.yahoo.com` | EGRESS_BLOCKED |
| `maps.roadtrippers.com` | EGRESS_BLOCKED |
| `en.wikipedia.org` | EGRESS_BLOCKED |
| `github.com` | **OK** — control, proves the allowlist |

Keyword search still functions, but it returns only result titles, URLs and
a machine-written gloss of them — never review bodies. A gloss is not a
review. Using one as a quote would have invented customer complaints and
attributed them to named local businesses, so nothing from it was kept.

Two facts incidentally confirmed by search result titles, usable only as
scale checks, not as complaint evidence:

- One Call Detailing, Yelp listing title: "635 Photos & 83 Reviews", 600 NE
  33rd St, Pompano Beach — <https://www.yelp.com/biz/one-call-detailing-pompano-beach>
- Mobile Detailers, Yelp listing title: "17 Photos & 47 Reviews", 4613 N
  University Dr, Coral Springs — <https://www.yelp.com/biz/mobile-detailers-coral-springs-8>

The README's "~571 reviews" figure for One Call Detailing is a Google count;
Yelp is a separate, much smaller pool.

---

## How to actually get this data

Three routes, cheapest first.

**1. Re-run with real egress.** Recreate the environment with a network
policy that genuinely allows `yelp.com` and `google.com`, then re-run this
task. This is the only route that costs nothing.

**2. Collect by hand, 60–90 minutes.** For each business, open the Google
Maps listing, set Sort → Lowest rating, and copy every review at 3 stars
and below; then the Yelp listing, filter to 1–3 stars, same. Paste verbatim
into `reviews-raw.md` under a heading per business, one block per review:

```
### One Call Detailing — Google Maps
**2★ — <name> — <month year>**
> <exact review text>
Source: <url>
```

Do not paraphrase while copying. The wording is the product — the exact
nouns customers reach for when angry are what the website copy has to
answer.

**3. Paid API.** Google Places API "Place Details" returns only five
reviews per place and cannot sort by rating, so it is not sufficient alone.
A SERP vendor with a Google Maps reviews endpoint (Apify, SerpApi,
Outscraper) returns the full set for a few dollars per business. Yelp's
official Fusion API returns three review excerpts only; full Yelp review
text needs a scraper and is against Yelp's terms.

## What to do once the text exists

Only then, and only from the collected text:

1. Tag each review with every complaint theme it contains — one review can
   carry several. Let the tags come from the reviews, not from a prepared
   list.
2. Rank themes by **number of distinct businesses** they appear across
   first, raw count second. A gripe that recurs at four of five competitors
   is a structural weakness in how the corridor operates and is worth
   building the offer around. A gripe at one business is that business's
   own problem and is worth nothing.
3. Only themes appearing across three or more of the five earn website copy.
   Each one becomes a promise on the site *and* a rule in operations that
   makes the promise true. A promise with no operating rule behind it
   generates the same review, about us.
4. Keep the source review beside each rule, so the reason for the rule
   survives after everyone forgets where it came from.

Step 3 is the discipline that matters. Copy that promises what operations
cannot deliver converts strangers into one-star reviewers.
