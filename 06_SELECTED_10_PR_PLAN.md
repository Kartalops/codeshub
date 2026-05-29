# 06_SELECTED_10_PR_PLAN — codeshub

## Selection Rationale
Selecting 10 PRs that are:
- All LOW risk
- All docs, content, or small tooling changes
- No code execution risk (pure snippets)
- No new dependencies
- Each independently mergeable
- Each verifiable without special environment

## Selected 10 PRs

### 1. C001 — docs: make language cards link to GitHub source
- **Linked Issue:** #352
- **Risk:** low
- **Diff Size:** ~30 lines
- **Target Files:** `docs/index.html`, `docs/js/main.js`
- **Test Plan:** Open `docs/index.html` locally, verify language cards link to correct GitHub folders
- **PR Title:** `docs: add GitHub source links to language category cards`
- **Status:** queued

### 2. C006 — docs: add Cash Register program in C++
- **Linked Issue:** #378
- **Risk:** low
- **Diff Size:** ~80 lines
- **Target Files:** `Cpp/CashRegister.cpp`
- **Test Plan:** Read the file to verify it compiles and is a valid C++ cash register implementation
- **PR Title:** `docs: add Cash Register program in C++`
- **Status:** queued

### 3. C002 — docs: add license and Hacktoberfest badges to README
- **Risk:** low
- **Diff Size:** ~5 lines
- **Target Files:** `README.md`
- **Test Plan:** Verify badges render correctly in GitHub preview
- **PR Title:** `docs: add license and Hacktoberfest badges to README`
- **Status:** queued

### 4. C003 — docs: update CONTRIBUTING.md directory structure
- **Risk:** low
- **Diff Size:** ~20 lines
- **Target Files:** `CONTRIBUTING.md`
- **Test Plan:** Read updated file, verify all language folders are listed and naming convention is clear
- **PR Title:** `docs: clarify directory structure in CONTRIBUTING.md`
- **Status:** queued

### 5. C012 — docs: add contribution flow for adding new languages
- **Risk:** low
- **Diff Size:** ~15 lines
- **Target Files:** `CONTRIBUTING.md`
- **Test Plan:** Read section, verify instructions are clear and complete
- **PR Title:** `docs: add guide for adding new language directories`
- **Status:** queued

### 6. C005 — docs: add DO NOT EDIT warning to site_data.json
- **Risk:** low
- **Diff Size:** ~2 lines
- **Target Files:** `docs/site_data.json`
- **Test Plan:** Open file, verify header comment is present
- **PR Title:** `docs: add auto-generated warning header to site_data.json`
- **Status:** queued

### 7. C004 — docs: add schema comments to generate_site_data.py
- **Risk:** low
- **Diff Size:** ~10 lines
- **Target Files:** `docs/scripts/generate_site_data.py`
- **Test Plan:** Read script, verify comments explain output schema clearly
- **PR Title:** `docs: add output schema documentation to generate_site_data.py`
- **Status:** queued

### 8. C015 — chore: add .gitignore for common IDE files
- **Risk:** low
- **Diff Size:** ~20 lines
- **Target Files:** `.gitignore`
- **Test Plan:** Verify .gitignore has standard entries (.vscode, .idea, .DS_Store, node_modules)
- **PR Title:** `chore: add .gitignore for common development files`
- **Status:** queued

### 9. C014 — docs: add good first issue guidance to CONTRIBUTING.md
- **Risk:** low
- **Diff Size:** ~10 lines
- **Target Files:** `CONTRIBUTING.md`
- **Test Plan:** Read section, verify examples are clear and helpful
- **PR Title:** `docs: add good first issue examples to CONTRIBUTING.md`
- **Status:** queued

### 10. C011 — test: add validation of generate_site_data.py output
- **Risk:** low
- **Diff Size:** ~15 lines
- **Target Files:** `docs/scripts/generate_site_data.py`
- **Test Plan:** Run script, verify it produces valid JSON with required fields
- **PR Title:** `test: add JSON schema validation to generate_site_data.py`
- **Status:** queued

## PR Sequence
1. C002 (badges — simplest, good first PR)
2. C005 (site_data.json comment — very safe)
3. C008 note: We SKIP C008 (typescript rename) — too risky for a snippets repo, could break existing links
4. C003 + C012 + C014 (CONTRIBUTING.md improvements — combine into logical PRs)
5. C001 (language card links — #352)
6. C006 (new C++ snippet)
7. C015 (.gitignore)
8. C004 + C011 (generate_site_data.py improvements)
9. C010 (_config.yml comment)

**Note:** Combined CONTRIBUTING.md improvements into C003/C012/C014 separately so each PR is focused and reviewable.

## Excluded Candidates
- **C008** (typescript → TypeScript rename) — SKIPPED: medium risk, could break existing links to `typescript/` folder
- **C013** (guide/configure.txt) — SKIPPED: unclear if intentional, don't want to remove without maintainer confirmation
- **C007** (Python project #358) — SKIPPED: #358 is vague ("Adding an Python project"), no specific details on what to add