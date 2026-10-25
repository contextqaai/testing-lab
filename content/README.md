# Teaching and creator kit

Status: draft teaching materials. Validate all exercises and current product behavior before recording or publishing. Use pinned app versions and real evidence. Do not promise capabilities based only on documentation.

## Flagship YouTube episode — 15 to 20 minutes

Working title: **Can an automated test catch this broken React payment flow?**

Opening narration: “Today we'll take a public React application, state what a transaction must do, run a test, and deliberately break the application. You can inspect the source and reproduce every step. This is an educational app with simulated transactions.”

0:00–1:00 — Open the exact fork and identify its upstream creators. Show the release and setup, including any manual preparation.

1:00–3:00 — Walk the flow manually once. State three assertions: selected recipient, exact amount, expected transaction history. Use synthetic users.

3:00–6:00 — Open your authenticated ContextQA workspace. Create/review the steps using the supported portal or MCP flow. Explain where human review was needed.

6:00–9:00 — Start execution. Show the actual verdict and the relevant assertion evidence. Distinguish setup time, edited waiting time and execution time.

9:00–12:00 — Switch to a separately identified broken variant. Keep the test unchanged. Show the failure, its evidence and what it proves. If a test passes unexpectedly, explain and investigate rather than hiding it.

12:00–15:00 — Show the app fix and rerun. Link both commits and reports. Locator repair and fixing a wrong business outcome are distinct lessons.

15:00–18:00 — Demonstrate supported code export/CI only if a clean independent run verifies it. Otherwise explain the current manual continuation plainly.

18:00–20:00 — Show how to begin on an authorized app of your own. Explain synthetic data, authenticated setup and destructive-action confirmation. End with the exact exercise link, not a sales-demo requirement.

Publish alongside: transcript, chapters, fixture version, app commits, generated test if available, actual result artifacts, setup limitations and corrections. Shorts: the assertion; the failure; the rerun. Do not turn an observed example into a general performance claim.

## Udemy course — proposed 120-minute curriculum

1. Orientation and supported setup — 10 minutes. Outcome: identify the app, runner, scenario and assertion.
2. HTML starter — 10 minutes. Outcome: add/filter/reload and assert persistence in a clean profile.
3. React transaction workflow — 20 minutes. Outcome: assert recipient, amount and history.
4. Angular workflow — 20 minutes. Outcome: create an article, verify authorship, comment and paginate.
5. Java/Spring workflow — 20 minutes. Outcome: create a pet/visit and assert correct ownership.
6. Regression diagnosis — 15 minutes. Outcome: separate app failure, locator failure and infrastructure error.
7. Verified export/CI and your own app — 15 minutes. Outcome: reproduce supported outputs independently; substitute a manual workflow if unavailable.
8. Capstone — 10 minutes. Outcome: design three assertions and catch a disclosed regression without following the instructor's exact test.

Each module needs prerequisites, fixtures, one exercise, expected observations, troubleshooting and an answer key based on actual execution. Keep the answer key out of the first learner page. Publish only after an unfamiliar reviewer reproduces the full course. Instructor, pricing, accounts and platform review remain open.

## Internal workshop — 30 minutes

5 minutes: source and assertion. 10 minutes: participant builds/runs a test. 5 minutes: diagnose a failing variant. 5 minutes: apply it to a team-relevant app. 5 minutes: teach back limitations.

Pass criterion: the participant can explain what an actual report proves, reproduce an assertion and name the next setup step for their own application. A watched recording alone does not count as completion.

## Creator brief

Choose a React/Angular, Java/Spring or testing educator whose audience includes hands-on practitioners. Ask for an independent walkthrough with visible source, one actual run, one disclosed regression and an attempt on an app of their own. Do not require a favorable verdict.

Suggested pilot scope to negotiate: one substantial video, two clips and a written recap. Supply a pinned release, synthetic fixtures, explicit assertions, known issues and technical help. Give every content piece a distinct attributed scenario link. Agree sponsorship disclosure, compensation, correction handling and footage reuse rights separately. No creator contact or payment is implied by this brief.

Evaluate qualified first-run completions, own-app completions, cost and support burden. Do not pay for positive claims, fake comments, stars or manufactured testimonials.

## Stack-specific series expansion

Modern developer playlist: .NET eShop, ASP.NET Core monolith, Spring Boot, MERN, Node API, Angular and Next.js. Modernization playlist: Java MVC/JSP versus Boot and paired Salesforce Visualforce/LWC behavior. Enterprise playlist: real Salesforce org exercises and the clearly scoped SAP Fiori/CAP web sample; ECC/S/4HANA/native SAP GUI episodes wait for actual sandbox/runner evidence. AI-builder playlist: bring a Lovable app, import/configure a Replit app, and validate a Vercel preview.

Each episode needs its own source, platform/runtime requirements, fixture, explicit assertion and actual report. Platform names are audience entry points, not claims of verified deployment. Migration episodes use matched business outcomes, not unsupported claims of automatic framework conversion. Do not market the current 120-minute outline as covering every added stack: publish modular playlists and separate beginner/enterprise courses.
