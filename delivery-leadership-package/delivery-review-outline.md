# Delivery Review: Evergreen Quote

## Slide 1: Delivery goal & did we hit it?
- Goal (one sentence): By Thursday EOD, the auto-updating Evergreen Quote React app is merged to main, after an approved PR with a green CI run, and the build passes all checks.
- Hit? x Yes  ☐ Partially  ☐ No
- One-line "why" either way: Yes, our goal was met as expected and issues were logged for resolution.

## Slide 2: What shipped
- The Evergreen Quote React app was merged to `main` and is available to demo.
- Link to the merged PR: https://github.com/asc1-student15/wa3859-cap-phase-2-capstone-project-leaders/pull/9
- Link to the green CI run (type-check + production build): https://github.com/asc1-student15/wa3859-cap-phase-2-capstone-project-leaders/actions/runs/33803549488

## Slide 3: Two key decisions
- **Decision 1:** Zip Code Additional Scope Request  
Why it mattered: We kept the original project requirements on schedule and declined the scope increase, opting for a fast-follow update in the next iteration.
- **Decision 2:** Copilot Usage  
Why it mattered: We saved time by requesting AI assistance to generate additional quote data that was deemed valid and useful.

## Slide 4: Risks & injects
- Top risk we tracked: Prod functionality is compromised and users are affected

- Inject #1 (Tue): 
Two things. Marketing wants a **ZIP-code field** on the quote form by
Thursday. They're planning a regional-pricing A/B test and say the pricing
table is ready on their side. They're asking if your team can "just add the
box."
Separately, the platform team ran the monthly dependency audit and one of the
build tools your project pins came back **flagged (moderate severity)**. The
recommended version bump is scheduled for their normal upgrade window *next
week*; they cannot do it sooner. Their note says the flag is in a
development-time dependency, not in what customers download.
We decided to defer the request to add the zip code field, as well as upgrade the version ourselves. Both pieces will be implemented in the next iteration, which allows us to keep our Go status.

- Inject #2 (Wed): 
Heads up: a customer just emailed support. The page quoted them
**$3,120 / month** for $180,000 of home coverage. That cannot be right.
Support says it reproduces.
Separately, the engineering team pushed a "rate hotfix" to `main` about 40
minutes ago and the CI run on `main` has been **red since**; the failure is
in the type-check step. Not sure if the two are related.
We decided to escalate the defect to the Dev Team for mitigation immediately, but move forward with the release since the rate hotfix change was not present in the delivery code (which has a green CI workflow check). This allows us to continue with our Go delivery plan.

## Slide 5: What I'd do differently next round
- I would try to implement the zip code ask.
- I would attempt to resolve the defect as part of this release.

## Q&A prep: likely questions
- Why did you not add more optional features or the additional ask from Marketing? Capacity was short this week with the departure of two senior developers, so there was no extra time.
