# Module 1 — Strategy: Meridian (The Field Gap)

_Completed in the Module 1 Lab Guide (Playing to Win cascade, hard no, OKR cascade, and AI pressure-test), reviewed and edited, then committed here._

**Scenario:** Meridian is a B2B construction project management platform built for enterprise complexity. Field superintendents and foremen never adopted it — they run on phone cameras and group texts instead. Challenge: make it indispensable to field teams without stripping the enterprise depth the largest customers pay for.

## Playing to Win cascade

**Winning aspiration**
Field superintendents and foremen trust Meridian as the fastest way to capture and escalate a jobsite issue, faster than dropping a photo in the crew group text — because logging it there gets them a faster answer, not more paperwork.

**Where to play**
Field superintendents and foremen at mid-market and enterprise general contractors already on a Meridian contract, starting with daily field documentation, RFIs, and punch-list/issue capture on active U.S. commercial job sites.

**How to win**
A camera-first, one-tap capture flow that is as fast as texting a photo, but automatically files it into the project record our enterprise buyers already depend on — turning the crew's fastest habit into the system of record instead of competing with it.

**Capabilities required**
World-class offline-first mobile capture (sub-3-second photo-to-post, works with no signal on site), automatic routing and tagging (project, location, trade), and fast return-value loops (status, approvals, RFI answers) that give foremen a reason to open the app again.

**Management systems**
Weekly field adoption rate (licensed field seats logging at least one item) and time-to-log reviewed by product and CS; monthly account-level usage review with our largest customers; quarterly review of field usage against the seats they are paying for.

## Hard no

We will not redesign the enterprise project console or its permissioning model to make it simpler for field use. We will win field adoption through a new capture layer, not by diluting the depth our largest, highest-paying customers rely on for compliance and reporting.

## OKR cascade

**Objective:** Make Meridian the fastest, most trusted way for field crews to capture and escalate jobsite issues, without changing what our enterprise customers already depend on.

**KR1:** Weekly active field users (foremen/superintendents logging ≥1 item): 18% to 60% of licensed field seats by Q3

**KR2:** Field-originated issues resolved within same-shift SLA: 34% to 70% by Q3

**KR3:** Job-site incidents first reported through informal channels (group texts/photos, not Meridian): 65% to under 20% by Q3

## AI pressure-test

**Which challenge from the AI is most valid, and why?**
The most valid challenge is the assumption that friction, not trust, is the real adoption barrier. Our capabilities section bets entirely on speed — a faster capture flow — but foremen may avoid logging issues in Meridian specifically because a timestamped, attributable record can be used against them in disputes or performance reviews. If that's true, a faster version of the same tool just makes the trust problem worse, not better. We haven't validated which barrier is dominant before committing capability investment to solving only the speed half of it.

**What would you change based on the pushback, and what would you defend?**
I'd change KR2: time-to-log measures tool speed, not a real business outcome, so I'd add a KR tied to something enterprise buyers actually pay for, like reduced dispute resolution time or rework hours tied to undocumented field issues. I'd also add a lightweight discovery step before building the capture layer, to test whether the barrier is friction or liability trust, since the two require different fixes. I'd defend the hard no about not redesigning the enterprise console — the AI's counterpoint that foremen may need minimal admin functions, like assigning or closing out an item, is fair, but that's a scoped exception inside the new capture layer, not a reason to touch the console our paying customers depend on for compliance and reporting.
