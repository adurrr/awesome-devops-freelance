# Changelog

All notable changes to the awesome-devops-freelance project.

Dates in YYYY-MM-DD format.

---

## [2026-05-31]

### Added
- Profile: `antonio-diaz-malt.md` — Spain ✅ verified (€400/day, Córdoba)
- Profile: `german-g-malt.md` — Spain 🔶 likely (€320/day, Madrid)
- `docs/ARCHITECTURE.md` — Architecture documentation extracted from PHASES.md
- `data/freelancer-profiles/SCHEMA.md` — Profile field schema and validation rules
- `.github/workflows/check-freshness.yml` — Automated stale content detection by "Last updated" dates
- `CHANGELOG.md` — This changelog

### Changed
- `AGENT.md` moved to `.github/AGENT.md` — removed root-level AI config file
- `research/methodology.md` moved to `docs/research/methodology.md`
- `research/paradigm-familiarization.md` moved to `docs/research/paradigm-familiarization.md`
- `data/freelancer-profiles/real/README.md` — count 85→87, verification summary updated
- `data/freelancer-profiles/README.md` — count synced to 87
- `PHASES.md` archived to `.github/PHASES.md` (historical planning); architecture docs now in `docs/ARCHITECTURE.md`
- `README.md` cross-references updated: `./research/` → `./docs/research/`
- `.github/workflows/weekly-update-check.yml` — search paths updated (`research/` removed)
- Hugo site now mounts root `docs/` directly instead of maintaining `site/content/docs/` copy
- Added `_index.md` files to root `docs/` subdirectories for Hugo section pages

### Fixed
- Hugo site duplication: root `docs/` and `site/content/docs/` are no longer separate copies

---

## [2026-05-29]

### Added
- README.md "Last updated": 2026-05-29
- Site homepage (site/content/_index.md) built from README.md content

---

## [2026-05-26]

### Added
- Research methodology document (docs/research/methodology.md — moved from research/ later)

---

## [Initial Commits — 2026-05-20 to 2026-05-25]

### Added
- Project initialization with AGPLv3 license
- README.md framework with curated tool lists
- PHASES.md project plan (10 paradigms, 7 phases)
- AGENT.md with AI agent instructions
- Research documents: all 13 paradigm deep dives
- Extended tool lists: all 12 category documents
- User-facing guides: how-to-use, how-to-contribute, freelance roadmap
- Freelancer profile analysis: 50+ profiles analyzed
- Academic references with SLRs from ACM, IEEE, arXiv
- Phase 5 automation: validate-links, weekly-update-check, stale issue management, Dependabot
- Phase 6 final review: cross-link validation, consistency pass
- Phase 7 Hugo documentation site with Book theme
- GitHub Actions deploy workflow for Hugo → GitHub Pages
- Custom styling with dark mode support
- 87 freelancer profiles in data/freelancer-profiles/real/
