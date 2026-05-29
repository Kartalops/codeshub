# 03_ISSUE_TRIAGE — codeshub

## Open Issues

| Issue | Type | Clarity | Repro Available | Existing PR? | Estimated Size | Risk | Selected? | Notes |
|-------|------|---------|-----------------|--------------|----------------|------|-----------|-------|
| #379 | enhancement | medium | no | no | small | low | yes | Add "Favorite" Option — UI feature for docs website |
| #378 | enhancement | high | no | no | small | low | yes | Add Cash Register Program in Cpp — new snippet |
| #358 | enhancement | medium | no | no | small | low | yes | Adding Python project — new snippet |
| #356 | enhancement | medium | no | no | small | low | yes | Python Project — new snippet |
| #352 | enhancement | high | no | no | medium | low | yes | Make code name clickable to view in GitHub — docs website link |
| #341 | enhancement | low | no | no | medium | low | no | "Meaningful codes into proper structure" — vague, no specific plan |

## Issue Details

### #352 — Make code name clickable to view in GitHub
- **Labels:** enhancement, help wanted, hacktoberfest-accepted, hacktoberfest
- **Type:** docs/website feature
- **Problem:** In the docs website (`docs/`), language cards don't link to the actual GitHub source
- **Size:** medium — involves `docs/index.html`, `docs/js/main.js`, `docs/site_data.json` generation
- **Selected:** yes — clear request, good for contributor visibility
- **Approach:** Add GitHub source links to language category cards in docs website

### #379 — Favorite Option for Languages
- **Type:** enhancement (docs website)
- **Problem:** Users can't bookmark/favorite languages in docs website
- **Size:** small
- **Selected:** yes — simple UI enhancement

### #378, #358, #356 — New Code Snippets
- **Type:** new content
- **Problem:** Missing C++ (cash register) and Python projects
- **Size:** small
- **Selected:** yes — these are exactly what the repo is for

## Recently Closed Issues (Reference)

| Issue | Type | Closed | Resolution | Notes |
|-------|------|--------|------------|-------|
| #375 | docs | 2025-10-22 | merged | Add Postfix configuration steps |
| #374 | config | 2025-10-22 | merged | Add transport_maps configuration |
| #373 | enhancement | 2025-10-22 | merged | pipe mail-box to bash script |
| #372 | config | 2025-10-22 | merged | Add configuration for mail source pipes |
| #371 | enhancement | 2025-10-22 | merged | email filtering and forwarding rules |
| #370 | enhancement | 2025-10-22 | merged | mail_to_api.sh forwarding emails to API |
| #351 | enhancement | 2025-10-06 | merged | oop concepts in java |
| #349 | bug | 2025-10-06 | merged | Languages not displaying on website (data field reference fix) |
| #347 | enhancement | 2025-10-06 | merged | QR_generator_and_reader.py |
| #346 | bug | 2025-10-06 | merged | Fix homepage language count display |

## Pattern Analysis
- Merged PRs are mostly: new code snippets, docs fixes, website display fixes
- Recent postfix/email files appear unrelated to core project (guide/configure.txt)
- No test coverage exists
- Hacktoberfest heavily used (labels: hacktoberfest, hacktoberfest-accepted)
- The `docs/` website fixes are welcome and get merged (#349, #346, #348)
- "good first issue" label exists (#322) but vague scope

## Selected for PR Planning
1. **#352** — Make code name clickable (docs website)
2. **New C++ snippet** — Cash register program (#378)
3. **New Python snippet** — as proposed in #358
4. **docs/ website** — Add better language card metadata display