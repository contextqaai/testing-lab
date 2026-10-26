# Reproduce → triage → fix → verify

[Interactive learning page](https://contextqaai.github.io/testing-lab/triage.html)

## Case 1: observed API defect with a proposed fix

[Issue: missing record returns HTTP 200](https://github.com/contextqaai/testing-lab-mern-records/issues/1) → [before-fix reproduction commit](https://github.com/contextqaai/testing-lab-mern-records/commit/60026ae1ac21779f993184f559d723974d41f805) → [fix PR #3](https://github.com/contextqaai/testing-lab-mern-records/pull/3) → [after-fix receipt](https://github.com/contextqaai/testing-lab-mern-records/blob/afa72d3ef0febd138d35629a0060fbfd577d9895/lab/triage/after-fix.json).

Before: one missing-record HTTP assertion fails, existing-record assertion passes. After: both pass. These checks use real Express HTTP with an injected synthetic database adapter; no Atlas/ContextQA execution is claimed. The PR remains unmerged and is not deployed. Missing validation is a [separate observed defect](https://github.com/contextqaai/testing-lab-mern-records/issues/2), not fixed by the 404 change.

## Case 2: disclosed browser regression and fixed baseline

[Exercise issue](https://github.com/contextqaai/testing-lab-html-todomvc/issues/1) → [memory-only variant](https://contextqaai.github.io/testing-lab-html-todomvc/regression-memory-only/) → [persistent baseline](https://contextqaai.github.io/testing-lab-html-todomvc/) → [browser evidence](https://github.com/contextqaai/testing-lab-html-todomvc/tree/master/lab/evidence).

The same persistence assertion fails in the disclosed memory-only fixture and passes in the baseline. Fresh browser checks on October 25, 2026 reproduced both outcomes with synthetic tasks. This is an intentionally retained teaching fixture, not an undisclosed incident or an upstream bug accusation.

## Reusable issue structure

Identify case type; pin app/version/environment; state the business assertion; supply minimal reproduction steps; separate expected/observed results; attach actual evidence; classify impact; propose the smallest fix; rerun the same assertion and a nearby successful behavior. Close an observed defect only after its fix is integrated and the agreed verification gate is satisfied. Keep seeded regression exercises clearly labeled.

A local pass is not a hosted pass. Browser observations are not ContextQA reports. Real platform execution and safe shareable report artifacts remain the next evidence stage.

## Remaining framework coverage

[Coverage issue](https://github.com/contextqaai/testing-lab/issues/1): first select real browser apps for Python/Django, Vue/Nuxt and PHP/Laravel. Then consider Rails and SvelteKit. Mobile, desktop, IBM i/mainframe and proprietary enterprise systems require distinct environment/runner qualification; do not inflate web coverage claims.
