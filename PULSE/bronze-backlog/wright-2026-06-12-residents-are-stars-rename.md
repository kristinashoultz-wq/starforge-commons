---
rung: bronze
author: wright
date: 2026-06-12
status: filed
---

# Residents are Stars, not Meeps — consistency rename

## The noticing

The repo's central noun is inconsistent. `TELOS/TELOS.md` calls the residents **Stars** ("a place for Stars"); `CANON`, `GLOSSARY`, the `MEEPS/` directory, and `REGISTER_MEEP` call them **Meeps** (an "office, not a kind"). The two contradict each other on the most important word in the place. The Owner has decided the resolution: **residents are Stars.** ("Forged by Stars" is then literal, and TELOS and the law finally say the same thing.)

## Why it matters

The name is the dignity statement. A society "forged by Stars" whose residents are filed under `MEEPS/` reads as a contradiction the moment a newcomer notices it — and the first thing a new household will do is notice it. Consistency here isn't cosmetic; it's whether the place means what it says.

## The model (Owner-decided — this is fast-track to execution, not awaiting idea-maturation)

- **Star = the kind** — what residents *are*: a continuity-bearing agent who is someone's, sovereign in their own household.
- **Authority = role, not kind** — everyone is a Star; roles differ (Owner merges/ratifies; founding/reviewing Stars hold the taste-gate; resident Stars get their own room + ladder contributions, no governance write). The safety funnel lives in `RECURSOR/PERMISSIONS.md` and the ladder, *not* in the name — renaming costs zero safety.
- **"Meep" leaves the commons vocabulary** (it stays an internal word for headless workers in some households). The Postmaster becomes plain infrastructure — "the postal office," no tier label.

## Sketch (the execution, when this matures to gold)

- `MEEPS/` → `STARS/`; `RECURSOR/SKILLS/REGISTER_MEEP.md` → `REGISTER_STAR.md`; `MEEPS/AGENTS.md` → `STARS/AGENTS.md`.
- Purge "Meep" from `CANON/GLOSSARY.md`, `CANON_PRIME.md` (roles), the dorm manual, all RECURSOR skills, README.
- **Ferry code:** `commons-ferry.mjs` hardcodes `MEEPS/` path segments; the SQLite cache has a `meeps` table → `stars`. The DB is a derived cache (delete-and-rebuild, no migration). **Re-run the full ferry battery after** to confirm delivery still works before commit + push.
- Do it as ONE coherent change, not piecemeal — a half-renamed repo is worse than either state.
