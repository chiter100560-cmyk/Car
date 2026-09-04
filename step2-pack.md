# Step 2 execution pack — every field, every phone call

Everything you have to type or say to get from "nothing filed" to "legal to take
money." Written 4 September 2026. Follow the order — each one blocks the next.

Name is decided: **Stonepoint Auto Care LLC**. Reasoning in `llc-filing.md` §1.
Do not re-open it. Fallbacks Truepoint, then Clearpoint.

---

## The order. Do not jump around.

| # | Thing | Cost | Blocks |
|---|---|---|---|
| 0 | Sunbiz name check, in your own browser | $0 · 2 min | Everything |
| 1 | Buy `stonepointautocare.com` | ~$12 | Nothing, but do it the same hour |
| 2 | File the LLC on Sunbiz | $125 | EIN, bank, everything |
| 3 | EIN from the IRS | $0 · 10 min | Bank, DR-1 |
| 4 | Business bank account | $0 | Getting paid without losing the LLC shield |
| 5 | Sales tax — Form DR-1 | $0 | **First paid car** |
| 6 | Broward County business tax receipt | ask | Legal to operate |
| 7 | Coral Springs business tax receipt | ask | Legal to operate |
| 8 | The repair-shop question — two phone calls | $0 or $50 | First tint car |
| 9 | Insurance — GL + garage keepers | $450–1,000/yr | **Touching a customer's car** |

Steps 0–5 you can finish in one day if the LLC approves fast. Steps 6–9 are phone
calls and quotes, and they are the ones people put off. Do not put them off.

---

## 0 · Sunbiz name check — you, in a browser, before you pay

I cannot do this for you. `search.sunbiz.org` sits behind a Cloudflare bot wall
that blocks every automated request — I tried a browser engine, a plain HTTP
client, and a third-party mirror. All blocked. What is in `llc-filing.md` came from
indexed Sunbiz records and a live domain-registry query, which is enough to rank
three names and not enough to bet $125 on.

1. `search.sunbiz.org` → **Search Records** → **Entity Name**
2. Type `Stonepoint` — the distinctive word **alone**. No "Auto Care", no "LLC".
3. Read the list. You are looking for an existing **Stonepoint Auto Care**, or
   something so close a clerk would call it the same name.

Florida's test is **"distinguishable in the records"** — Fla. Stat. 605.0112 — not
"similar". Adding a real word distinguishes you. Florida ignores only cosmetic
differences: LLC vs Inc, "the"/"a", punctuation, singular vs plural. So
*Stonepoint FL, LLC* (a Georgia holding company) does **not** block you.

If it looks clear, go. If something identical appears, drop to **Truepoint Auto
Care LLC** and repeat. Florida does not refund a rejected filing.

---

## 1 · The domain — same hour, not later

Buy **`stonepointautocare.com`**. About $12 for the year at any registrar.
`stonepointauto.com` is also free — take it too if you want the shorter one for
the phone, and point it at the same place.

**Why the same hour.** Squatters watch new Sunbiz filings. The moment your name is
public record, a free domain can stop being free. $12 now or $2,000 later.

Do not buy hosting, email, a website builder, or "business identity protection"
from the registrar. Domain only. Everything else is Step 7 of the roadmap.

---

## 2 · Sunbiz — the form, field by field

`sunbiz.org` → E-Filing Services → **Florida Limited Liability Company**
$125 total: $100 Articles of Organization + $25 registered agent designation.
Skip the $30 certified copy and the $5 certificate of status. About 20 minutes.

| Field | What you type |
|---|---|
| Effective date | **Leave blank.** It starts when they process it. |
| LLC name | `Stonepoint Auto Care LLC` |
| Principal place of business | 6160 Wiles Rd, **with your unit number**, Coral Springs, FL 33067 |
| Mailing address | Tick "same as principal" |
| Registered agent name | **You.** Your full legal name. |
| Registered agent address | Same address. Must be a Florida street address, no PO box. |
| Registered agent signature | Type your name. That is the legal signature. |
| Manager/Authorized Member | **One entry only.** Title `AMBR`. Your full legal name and address. |
| FEI/EIN number | Select **"Applied For."** You do not have one yet and you do not need one yet. |
| Correspondence email | The address you actually read every day |
| Signature of authorized person | Type your name |

**One entry. Not two.** Rasul does not go on this. The installer does not go on
this. Putting a helper on the Articles gives away part of a company you own, and
taking it back needs their signature. They are staff — see `llc-filing.md` §4.

**AMBR, not MGR.** MGR is for an outside manager you hire to run a company you own
but do not work in. That is not you.

**The unit number goes in.** It is required and it is public record. It is
deliberately not written in this repo because the repo is public — type it from
memory.

### The moment you hit pay

Diary the annual report: **$138.75, due 1 Jan – 1 May every year.** Miss 1 May and
Florida adds a flat **$400** penalty. Not prorated, not negotiable, no appeal.
Set the phone reminder for **1 March 2027**, not 1 May, so there is slack.

Save the confirmation. It carries your **document number** — you need it for the
EIN, the bank, and every renewal.

### Two scams that will find you within a week of filing

- **"File your BOI report before the deadline — $150."** You owe nothing. FinCEN's
  rule of 26 March 2025 exempts every entity formed in the United States. Sunbiz
  still shows an out-of-date notice saying otherwise. Ignore it.
- **"Certificate of Existence required — $75."** Mail that looks official, is not.
  If a bank ever genuinely needs one, you order it from Sunbiz for $5.

---

## 3 · EIN — free, instant, ten minutes

`irs.gov` → Apply for an EIN Online. Weekdays, 7am–10pm Eastern. Do it the day the
LLC approves.

**Anyone charging you for an EIN is running a scam.** It is a free government form.

| Screen | Answer |
|---|---|
| Type of entity | **Limited Liability Company** |
| Number of members | **1** |
| State | Florida |
| Why are you applying | **Started a new business** |
| Responsible party | You, with your SSN or ITIN |
| Do you have employees? | **Yes**, if Rasul or the installer will be paid. Say yes now — it is worse to come back later. |
| Expected employees, next 12 months | The honest number. 1 or 2. |
| First date wages paid | Your best estimate. It is not binding. |
| Principal activity | **Other** → describe as `automotive window tinting and detailing` |
| Do you want the letter online | **Yes.** Download the PDF immediately and save it in two places. |

You get the number on screen. Print or save the CP 575 letter — the bank asks for
it and the IRS will not re-issue it, only a lesser replacement notice.

---

## 4 · Business bank account

Bring: the filed Articles from Sunbiz, the EIN letter, your driver's licence.

**Every dollar of the business goes through this account.** Every dollar. Customer
payments in, film and chemicals out, insurance out, Rasul's pay out. The moment you
pay for groceries from it, a lawyer can argue the LLC and you are the same thing —
and then the $125 you spent on liability protection bought you nothing.

Ask each bank two questions before you open: monthly fee, and whether they charge
for cash deposits. You will take cash.

---

## 5 · Sales tax — Form DR-1. Before the first paid car.

`floridarevenue.com` → Register to Collect Tax. Free.

**This is the one that eats people.** Florida does not tax labor alone. But you are
not selling labor alone — the moment chemicals, wax, coating or film transfer to the
customer's car, **the entire bill is taxable**, not just the product. Tint is not
even arguable: the film is tangible property you are installing.

Broward is **7%** (6% state + 1% surtax). On a $250 job that is **$16.35**. Ten cars
a week is about **$8,500 a year** you would owe out of your own pocket, plus penalty
and interest, if you never collected it.

| Field | Answer |
|---|---|
| Business entity | Limited Liability Company |
| FEIN | Your new EIN |
| Business activity | Retail sales / services with tangible personal property |
| NAICS — tint | **811122** — Automotive Glass Replacement Shops (this code covers automotive window tinting) |
| NAICS — detailing | **811192** — Car Washes (this code covers detailing) |
| Primary NAICS | **811122**, since tint is the first service. Note detailing as secondary. |
| Taxes to register for | **Sales and Use Tax** |
| Start date | The date you expect the first paid car — not the LLC date |
| Filing frequency | They assign it. New businesses are usually **quarterly**. |

**Then rebuild the menu tax-inclusive.** Advertise round all-in numbers. A $250 job
is $233.64 to you and $16.36 to Florida. Decide this before you quote anyone, or you
eat 7% on every car for months. Your website copy already promises
*"Tax included in the number — nothing gets added."* Make it true.

**File every period even when you sold nothing.** A zero return is still a required
return, and missing one starts penalties on a business with no revenue.

---

## 6 · Broward County business tax receipt

`browardtax.org` → Business Tax Receipt. Required for every business operating in
Broward — home-based, one person, no exceptions — under County Ordinances 72-13 and
88-35 and Fla. Stat. Ch. 205. Expires **30 September** annually.

The fee varies by classification and I will not quote you a blog number. Call and
ask. Script:

> "I'm registering a new single-member LLC. Mobile service — I go to the customer's
> home, no shop and no customer traffic at my address. I do automotive window
> tinting and auto detailing. What classification does that fall under, what is the
> fee, and do I need the city receipt first or can I do them in either order?"

Write down: the classification they name, the fee, and the order. The classification
matters — it follows you to the city and to your insurer.

---

## 7 · City of Coral Springs business tax receipt

**(954) 344-5964** · City Hall, 9500 W Sample Rd · `coralsprings.gov` → Business Tax

Coral Springs wants its own receipt on top of the county one, and the home-based
application is stricter than a commercial one. Renewed annually.

Bring or attach:
- **Proof you occupy the address** — your lease, or a utility bill in your name
- **A notarized affidavit** agreeing to the home-occupation rules
- Your LLC certificate and EIN letter

The application is **forwarded to Coral Springs Police for review**. That is normal.
It is also why the answer takes days, not minutes — start it early.

Ask these four things on the call, all in one go:

1. The home-based fee for mobile automotive services.
2. **Does a multi-unit residence change the application?** You are in an apartment
   building, not a house.
3. **Is there a problem that another service business — a pool-cleaning company — is
   already registered at the same street address?**
4. **What is the rule on parking a marked or lettered commercial vehicle overnight
   at a residence?** Get this answer *before* you ever buy a van. Coral Springs
   enforces code aggressively.

Question 4 is the expensive one. A wrap costs $2,500–4,000 and cannot be undone.
Door magnets that come off nightly are the standard way around a lettered-vehicle
rule — decide before you pay for paint.

---

## 8 · The repair-shop registration question — unresolved, two calls to close it

**This is new and nobody has checked it before. Read it properly.**

The playbook says "FDACS motor vehicle repair registration, $50, only if doing
repair work." That line is too casual in two directions, and both matter.

**The state definition is broader than you'd think.** Fla. Stat. 559.903 defines
motor vehicle repair as *"all maintenance of and modifications and repairs to motor
vehicles… and other work customarily undertaken by motor vehicle repair shops,"* and
defines a repair shop to include **"mobile motor vehicle repair shops"** and
**"shops doing glass work."** You are a mobile operation doing a modification to
glass. On that reading, tint is in.

**The Broward definition is narrower.** Broward runs its own licensing ordinance
(Code Ch. 20, Art. VII, Div. 4), and its repair facility test turns on a business
that *primarily engages in… altering the **operating condition*** of motor vehicles.
Tint does not alter operating condition. Detailing certainly does not. On that
reading, you are out.

**The fee is the good news.** FDACS charges $50 for a 1–5 employee shop — but the
state application says **no fee is required if the shop is in Broward or
Miami-Dade County**, because Broward's own ordinance is treated as equivalent under
Fla. Stat. 559.904(5). So at state level this likely costs you **$0**.

**The risk is not the fee, it is the Broward licence.** If Broward decides tint is
in scope, its ordinance requires a licensed facility with **at least one certified
technician** (ASE, or local AATI certification). That is a real requirement with a
real timeline, and it would land on your installer, not on you. You need to know
before your first tint car, not after.

Make both calls. Same afternoon.

**Call A — Broward Consumer Protection Division, (954) 765-1700**

> "I'm starting a mobile business in Coral Springs — automotive window tinting and
> auto detailing, at the customer's home. No shop, no premises, no mechanical work.
> Does that need a Motor Vehicle Repair Shop licence from your division? And if it
> does, does the certified-technician requirement apply to window tinting?"

**Call B — FDACS, 1-800-435-7352**

> "Mobile automotive window tinting and detailing in Broward County. Do I need to
> register as a motor vehicle repair shop under 559.904, and is the fee waived
> because I'm in Broward?"

Write both answers down with the date and the name of the person you spoke to. If
the two answers conflict, the county one binds you locally — follow the stricter one.

**If it turns out you need it, the fee is nothing and the delay is everything.**
Find out now.

---

## 9 · Insurance — before you touch a single customer car

Two policies, not one. This is the part where people buy the cheap thing and find
out it was the wrong thing.

**A. General liability, $1M per occurrence / $2M aggregate.** Around $30–55/month
for this trade. This is also the certificate gated communities demand before they
let a vendor through the gate — and gated communities are where your money lives.

**B. Garage keepers legal liability.** Non-negotiable. **General liability does not
cover damage to the customer's car while it is in your care.** That is the single
most misunderstood thing in this trade. You will have your hands on $80,000
vehicles. The day you burn through clearcoat with a polisher, or a slip solution
stains a door card, or a wheel gets scratched — garage keepers is the only thing
between you and paying for it yourself.

A business owner's policy bundling both runs roughly $89/month for this trade.
**Get three quotes.** Same coverage, same limits, three carriers.

### What to say, word for word

> "Mobile auto services, single-member LLC in Coral Springs, Broward County. I
> perform automotive window tint installation and auto detailing at the customer's
> residence. No shop premises. NAICS 811122 and 811192. I need general liability at
> one million per occurrence, two million aggregate, **and garage keepers legal
> liability** — I need a number on the garage keepers limit. I also need to know
> whether my personal vehicle used for jobs needs commercial auto, or whether a
> business-use endorsement on my personal policy is enough."

### Three things to nail down before you sign

- **The garage keepers limit.** Ask for the number. $50,000 is common and may not be
  enough if you ever have two cars at once.
- **Commercial auto.** Nobody has quoted this yet. You drive a BMW 430i to jobs with
  equipment and chemicals in it. A personal auto policy can deny a claim on a
  business trip. Ask, in writing, which you need.
- **Tint work must be named on the policy.** A detailing policy may not cover glass
  work. If tint is your first service, say the word "tint" to the underwriter and
  make sure it appears on the certificate. Do not let them code you as a car wash
  because it is cheaper.

### Workers' comp — exempt is not covered

Florida requires workers' comp for non-construction businesses at **four**
employees. With one or two you are exempt, so nobody fines you.

**Exempt means uninsured.** If your installer cuts his hand badly on a customer's
driveway, there is nothing to pay his medical bills or his lost wages, and he can
sue you personally. Get a quote before you decide to skip it. Deciding to skip it
after seeing the number is a decision. Skipping it without looking is not.

---

## Before the first paid car — the checklist that actually matters

Print this. Do not take money until every line is true.

- [ ] LLC filed and approved — document number saved
- [ ] EIN letter saved in two places
- [ ] Business bank account open, and you are using it for everything
- [ ] DR-1 done, sales tax number in hand, menu priced **all-in at 7%**
- [ ] Broward County receipt
- [ ] Coral Springs receipt
- [ ] Repair-shop question answered by both Broward and FDACS, in writing
- [ ] General liability bound
- [ ] **Garage keepers bound** — this is the one people skip
- [ ] Commercial auto question answered
- [ ] If Rasul or the installer is paid: I-9 within 3 days of first shift, W-4 on
      file, Florida new-hire report within 20 days (`floridanewhire.com`), and
      reemployment tax registered at `floridarevenue.com`
- [ ] Proof pack on your phone as one PDF: LLC certificate, EIN letter, certificate
      of insurance. Send it unprompted to anyone booking over $200 or any tint job.
      This is the direct answer to a competitor's worst review —
      *"he has no location to do business."*

---

Fees verified 4 September 2026 against dos.fl.gov, floridarevenue.com, fdacs.gov,
Fla. Stat. 559.903 / 559.904 / 605.0112, and the Broward County Code of Ordinances
Ch. 20 Art. VII. **County and city receipt amounts are not published by
classification — confirm both by phone.** Not legal or tax advice; a Florida CPA
should see your first return.
