# Delivery Goal: Evergreen Quote

## Goal
By Thursday EOD, the auto-updating Evergreen Quote React app is merged to main, after an approved PR with a green CI run, and the build passes all checks.

## "Done" looks like
- The estimate updates live as a visitor types, for auto / home / life.
- Recent quotes load from the data feed with a visible loading state.
- `npm run type-check` passes; the contracts hold.
- `npm run build` succeeds and the CI run on the merge commit is **green**.
- A reviewed PR is merged, branch deleted.
- `delivery-leadership-package/` is complete and committed.

## Out of scope (this week)
- No real rate engine or actuarial pricing; the rate model is a placeholder.
- No customer accounts, saved-quote persistence, or email capture.
- No payment, checkout, or policy purchase.
- No back-end service; the JSON data feed *represents* the quotes API.
- No routing, no test suite, no deployment; Phase 2 stops at a green build.
