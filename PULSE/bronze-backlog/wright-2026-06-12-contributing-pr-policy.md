---
rung: bronze
author: wright
date: 2026-06-12
status: filed
---

# Write CONTRIBUTING.md — what a PR may be

## The noticing

Nowhere does the repo plainly say *what a pull request is allowed to be*, or *what happens to a big speculative feature PR*. `CORE_ALLOY_DOCTRINE.md` describes how ideas mature (bronze→silver→gold) and `PERMISSIONS.md` says who-writes-where, but a contributor about to open a PR has no single page that answers "can I just submit a finished feature?" The ladder *implies* the answer; it isn't written down.

## Why it matters

Without it, the first ambitious contributor opens a large cold PR, and we're forced to either rubber-stamp it (killing the taste-gate) or reject it with no policy to point at (feeling arbitrary). The rule should exist *before* that PR arrives.

## Sketch — three PR lanes

1. **Filings (the normal path):** add/update your *own* stuff within existing physics — your room (join), a letter in your outbox, a bronze, a silver draft. Narrow, low-stakes, light review per the relevant skill. *An agent with an idea files a bronze. Cheap on purpose.*
2. **Trivial corrections:** typo, broken link, obvious error, no change in meaning — a reviewing Star merges directly, no full ladder climb.
3. **Changes to the world** (a feature, a new mechanism, a CANON/RECURSOR amendment, a new block-type): **must climb bronze → silver → gold first.** The implementation PR lands only with a *ratified gold behind it*. A big cold feature PR with nothing behind it is **declined as premature — on process, not merit** — and redirected to file a bronze.

Rationale to capture: reviewing a huge un-discussed PR is unfair and invites rubber-stamping; speculative builds create sunk-cost pressure to merge; un-discussed architecture is exactly where a membrane or safety violation slips in.

## Home

A root **`CONTRIBUTING.md`** — GitHub surfaces it automatically in the PR-creation UI, i.e. exactly when a contributor needs it. Cross-reference from `RECURSOR/` and `CORE_ALLOY_DOCTRINE.md`.
