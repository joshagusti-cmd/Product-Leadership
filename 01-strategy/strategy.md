# Module 1 - Strategy: Meridian (The Field Gap)

> First-pass draft. The lab guide asks you to try your own product thinking first and use AI only as a pressure-test, not a replacement - treat everything below as a starting point to react to, argue with, and rewrite in your own words before it counts as your submission.

**Scenario:** Meridian is a B2B construction project management platform built for enterprise complexity. Field superintendents and foremen never adopted it - they run on phone cameras and group texts instead. Challenge: make it indispensable to field teams without stripping the enterprise depth the largest customers pay for.

## Playing to Win cascade

**Winning aspiration**
A foreman documents the job site faster with Meridian than by texting a photo to the crew group chat - and stops needing the group chat at all. Winning is measured in what the field team feels (this is quicker than texting), not in an internal adoption dashboard.

**Where to play**
Field crews - foremen and superintendents - at the mid-to-large general contractors who already pay for Meridian's enterprise tier. North America initially, riding the existing enterprise install base rather than new-logo acquisition. Use case: daily field documentation (progress photos, punch lists, safety checks) - the narrow slice of the job field teams already capture on their phones, not the full PM suite.

**How to win**
Photo-first capture that beats opening the camera roll and texting the group chat: point, shoot, done - no required data entry. The app extracts structured records (location, trade, date, likely category) from what was already an ordinary photo action, so the enterprise data the office needs arrives as a side effect of what the crew was doing anyway. Competing field tools ask for forms-first entry designed around office/PM personas, which is exactly why crews abandon them for texting.

**Capabilities required**
Build in-house: sub-2-tap capture, offline-first sync (jobsites have poor connectivity), automatic metadata tagging. Buy or partner: computer-vision/OCR for auto-tagging rather than building it from scratch; an SMS bridge so a foreman can move between texting and the app mid-rollout without losing momentum.

**Management systems**
Metrics: weekly active foremen (not just PM/admin logins), captures-per-crew-per-day against the prior group-text baseline, time from capture to office visibility. Ritual: a monthly field-adoption review, separate from the existing enterprise renewal/QBR cadence and owned by a dedicated field-adoption PM, not the enterprise account team.

## Hard no

We will not require a foreman to fill in any structured field before a photo or note saves. If capturing something takes more taps than texting it, field adoption fails - so anything needing a required dropdown or field at capture time stays out of the field flow, even where the office and enterprise reporting would prefer more complete data. Speed and simplicity at the point of capture wins over office-side data richness.

## OKR cascade

**Objective:** Make Meridian the fastest way for a foreman to document the job site - faster than the group text they use today.

**KR1:** Weekly active field users (foremen/supers actually opening the app) grows from baseline to 40% of enterprise seats within two quarters.

**KR2:** Median time from photo capture to visible-in-office-dashboard drops to under 5 minutes for 90% of captures (from effectively never, since today it travels by text).

**KR3:** Self-reported "I'd rather use this than text the group chat" among surveyed foremen reaches 60%+ after rollout.

## AI pressure-test

Run against the cascade above using the lab's skeptical-Chief-Strategy-Officer prompt.

1. **Biggest assumption that could be wrong:** that zero-structure capture still produces data clean enough for enterprise reporting. Unstructured photos may not reliably become the punch lists, RFIs, and safety records the office needs - the hard no could just move the failure from field adoption to office-side uselessness, rather than solving it.
2. **The question a board member would ask that isn't answered yet:** if a foreman can save a photo with zero structure, how does raw field volume become the audit-ready daily log a GC needs for a billing dispute - and what's the evidence that automatic tagging is accurate enough to hold up outside a demo?
3. **KRs that are outputs disguised as outcomes:** KR2 (capture-to-visibility latency) measures the pipe, not a changed behavior or created value. It's closer to a system-performance output than a customer or business outcome.
4. **The hard no worth reconsidering:** "zero required fields, ever" may be a false binary - one lightweight, single-tap trade/category chip (not a form) could cost negligible friction while making auto-tagging meaningfully more reliable.
5. **Strategy or wish list:** strategy - there's a real differentiator (photo-first, zero-form capture) and a named trade-off (office completeness). But the auto-tagging accuracy assumption and KR2 are soft enough that it isn't fully stress-tested yet.

**Harsher pass (a competitor's strategy team):** a rival building a bare "just take a photo" app would argue Meridian's enterprise identity is itself the adoption barrier - a foreman who's never opened Meridian won't discover a stripped-down field mode buried inside an enterprise PM tool. A standalone app that syncs data into Meridian could win the "first open" moment that actually decides adoption.

**Which challenge is most valid, and why:** #1/#2 together - the assumption that zero-structure capture still yields office-usable data is load-bearing. If auto-tagging isn't reliable, the hard no doesn't protect focus, it just delays the failure to the office side.

**What I'd change vs. defend:** Defend the hard no on required fields at capture time - that stays zero-friction. Change the capabilities list to explicitly require a confidence-scored auto-tagging pipeline with a fast, optional office-side triage/correction step (not a mandatory field for the foreman, but a quick pass for whoever processes the daily digest). Also change KR2 from a latency metric to a downstream business outcome - e.g., reduction in office hours spent reconciling field documentation, or fewer disputed change orders traced to missing field records.
