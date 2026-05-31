# Architecture Guide

> **Purpose**: Documents the project's structure, principles, and maintenance strategy. This is a living reference for contributors and maintainers.

**Last updated**: 2026-05-31 (restructured docs/)

---

## 🧭 Core Principles

1. **Accuracy over breadth** → Fewer entries, higher quality, verified information
2. **Freelancer-first** → Every entry answers "Why does this matter for freelancers?"
3. **Progressive disclosure** → README = summary; docs/paradigms = deep detail; docs/tools = full comparisons
4. **Anti-hallucination** → Every claim traced to source; cross-referenced data; explicit uncertainty markers
5. **Living document** → Monthly review cycle; community contributions welcome

---

## 📐 Directory Structure

```
awesome-devops-freelance/
├── README.md                        ← Curated list (summary, navigation, top tools)
├── LICENSE                          ← AGPL v3
├── CONTRIBUTING.md                  ← Contribution guidelines
├── CHANGELOG.md                     ← Change log
├── docs/
│   ├── ARCHITECTURE.md              ← This file
│   ├── get-started/                 ← Entry-level guides
│   │   ├── how-to-use-this-list.md
│   │   └── freelance-devops-roadmap.md
│   ├── paradigms/                   ← Deep dives
│   │   ├── paradigm-familiarization.md
│   │   ├── landscape/               ← 9 paradigm landscape docs
│   │   │   ├── devops.md
│   │   │   ├── devsecops.md
│   │   │   ├── dataops.md
│   │   │   ├── mlops.md
│   │   │   ├── aiops.md
│   │   │   ├── finops.md
│   │   │   ├── llmops.md
│   │   │   ├── platform-engineering.md
│   │   │   └── sre.md
│   │   ├── cncf-landscape-analysis.md
│   │   └── academic-references.md
│   ├── tools/                       ← Detailed tool references (12 documents)
│   │   ├── ci-cd-tools.md
│   │   ├── iaac-tools.md
│   │   ├── container-orchestration.md
│   │   ├── observability-monitoring.md
│   │   ├── security-devsecops.md
│   │   ├── gitops-tools.md
│   │   ├── platform-engineering.md
│   │   ├── ai-for-devops.md
│   │   ├── cost-management-finops.md
│   │   ├── mlops-llmops-tools.md
│   │   ├── messaging-streaming.md
│   │   └── sre-tools.md
│   ├── careers/                     ← Freelancer career data
│   │   └── freelancer-profile-analysis.md
│   └── reference/                   ← Project reference docs
│       ├── methodology.md
│       ├── research-review-notes.md
│       └── how-to-contribute.md
├── data/                           ← Machine-readable data
│   └── freelancer-profiles/
│       ├── real/                   ← 87+ individual profile files
│       ├── README.md               ← Profile index (root)
│       ├── SCHEMA.md               ← Profile field schema
│       └── profiles.json           ← Structured dataset
└── .github/                        ← GitHub automation
    ├── AGENT.md                    ← AI agent instructions
    ├── PHASES.md                   ← Historical project plan (archived)
    ├── workflows/
    │   ├── deploy-site.yml         ← Hugo → GitHub Pages deploy
    │   ├── validate-links.yml      ← Monthly + PR link validation
    │   ├── weekly-update-check.yml ← Weekly stale content detection
    │   ├── check-freshness.yml     ← Content freshness by date metadata
    │   └── stale.yml               ← Auto-close stale issues/PRs
    ├── ISSUE_TEMPLATE/
    │   ├── add-tool.md
    │   └── update-resource.md
    ├── PULL_REQUEST_TEMPLATE.md
    └── dependabot.yml              ← Weekly Action dependency updates
```

### Justification for Each Component

| Component | Justification |
|-----------|---------------|
| **README** (curated list) | Primary entry point. Must be scannable in < 30 seconds. Contains top tools, quick navigation, and paradigm overview. |
| **Paradigm docs** (docs/paradigms/) | Deep references for when a user needs to go beyond the summary. Each is a standalone document for a specific paradigm. |
| **Tool lists** (docs/tools/) | Full tool comparisons with licensing, pricing, and freelance relevance. Allows README to stay concise. |
| **Freelancer analysis** | Distills real-world patterns from 87+ freelancer profiles. Actionable insights for positioning and pricing. |
| **Academic references** | Grounds the project in research. Optional for most readers but essential for credibility and future work. |
| **Methodology doc** | Documents validation process. Critical for anti-hallucination and trust. |
| **GitHub workflows** | Ensures quality over time. Link validation prevents rot. |

---

## 🔬 Anti-Hallucination & Quality Assurance Strategy

### Tier 1: Prevention (Design-time)

1. **Source tagging**: Every claim tagged with source type:
   - `[SOURCE: Perforce 2026]` = Industry report
   - `[SOURCE: arXiv:2604.16371]` = Academic paper
   - `[SOURCE: CNCF Landscape]` = Official tool listing
   - `[SOURCE: GitHub Stars]` = Verified on GitHub

2. **Uncertainty markers**: Explicit language for uncertain data:
   - "~25% market share" (= approximate)
   - "According to [source]" (= not direct knowledge)
   - "Sparse evidence" (= limited backing)
   - "Industry consensus suggests" (= qualitative observation)

3. **Cross-referencing**: Every market claim cross-checked with 2+ sources before inclusion

4. **Edition dating**: Every document includes "Last updated: YYYY-MM-DD"

### Tier 2: Detection (Review-time)

1. **Monthly review cycle**: First week of every month
2. **Link checking**: Automated check for dead/broken URLs
3. **Community QA**: Issue template includes "Source for this claim" field
4. **Peer review**: Before major changes, at least 1 community review

### Tier 3: Correction (Post-release)

1. **Correction log**: `CHANGELOG.md` tracks all corrections
2. **Retraction policy**: If a claim is found incorrect, mark with ~~strikethrough~~ and add note
3. **AI hallucination handling**: If AI-generated content identified, remove and flag in changelog
4. **Deprecation notices**: Tools that are deprecated get `⚠️ DEPRECATED` notice

### AI Usage Policy

- AI is used for: draft generation, cross-referencing, summarization
- AI is NOT used for: inventing tools, creating fake citations, fabricating metrics
- All AI-assisted content is verified against primary sources before inclusion
- Generated code examples are treated as "pseudocode" and verified by running them
- Freelancer analysis data is sourced from real platform profiles, not generated

---

## 📊 Success Metrics

| Metric | Target (3 months) | Target (1 year) |
|--------|-------------------|-----------------|
| GitHub stars | 100+ | 500+ |
| Paradigm documents | 12 | 15+ |
| Tool lists | 12 | 15+ |
| Open issues/PRs responded | < 48h | < 24h |
| Link rot | < 2% | < 1% |
| Community contributors | 3+ | 10+ |
| Monthly active users (est.) | 500+ | 2000+ |

---

## 🔄 Maintenance Plan

### Monthly Tasks
1. Run link checker → fix broken URLs
2. Review new tools released in each category (CNCF updates, GitHub trending)
3. Update tool statuses (graduated/incubating/deprecated)
4. Check for new freelance platforms or rate changes
5. Respond to open issues and PRs

### Quarterly Tasks
1. Major research review → update each research document
2. Freelancer rate survey → refresh rate data
3. CNCF landscape sync → update with new graduated/incubating projects
4. Academic literature search → add new SLRs and papers
5. Content audit → remove stale entries, add new ones

### Annual Tasks
1. Complete re-evaluation of all Ops paradigms
2. Major State of DevOps report analysis (Perforce, CNCF)
3. Freelancer profile re-analysis (refresh sample)
4. Platform comparison update (Toptal, Upwork, Arc.dev, etc.)
5. Roadmap update for next year

---

## 🛡 Risk Management

| Risk | Impact | Probability | Mitigation |
|------|--------|-------------|------------|
| Tool deprecation | Medium | High | Quarterly review; deprecation notice system |
| Rate data becomes outdated | Medium | High | 6-month refresh cycle |
| New Ops paradigm emerges | Medium | Medium | Flexible structure tolerates new categories |
| Community contributions are low | Low | Medium | Proactive outreach; reasonable first issues |
| Link rot (many broken URLs) | High | High | Automated monthly link checker |
| Academic sources paywalled | Low | High | Cite open-access versions when possible |
| AI hallucination in content | High | Low | Source tagging; cross-referencing; community review |

---

## 📁 File Map

All 28+ documentation files across the project, organized by section:

### Paradigms (docs/paradigms/)
- `paradigm-familiarization.md` — Entry-level overview of all Ops paradigms
- `landscape/` — 9 paradigm landscape docs (2026)
  - `landscape/devops.md` — Core DevOps trends, platform engineering, GitOps, IaC
  - `landscape/devsecops.md` — Shift-smart security, AI-driven preemptive security
  - `landscape/dataops.md` — Data pipelines, data versioning, quality
  - `landscape/mlops.md` — ML lifecycle management, model registry
  - `landscape/aiops.md` — AI for IT operations, self-healing
  - `landscape/finops.md` — Cloud cost management, chargeback
  - `landscape/llmops.md` — LLM operations, RAG systems, guardrails
  - `landscape/platform-engineering.md` — Internal developer platforms, Backstage
  - `landscape/sre.md` — SLI/SLO frameworks, error budgets, incident management
- `cncf-landscape-analysis.md` — All CNCF projects mapped by maturity
- `academic-references.md` — SLRs and papers for each paradigm

### Tools (docs/tools/)
- `ci-cd-tools.md` — 15+ CI/CD tools with comparison, pricing
- `gitops-tools.md` — ArgoCD vs Flux, multi-cluster GitOps
- `iaac-tools.md` — 15+ IaC tools, comparison matrix
- `container-orchestration.md` — 12+ orchestration tools, managed K8s
- `observability-monitoring.md` — 18+ observability tools, stack recommendations
- `security-devsecops.md` — 20+ security tools, compliance
- `sre-tools.md` — 25+ SRE tools, incident management, chaos engineering
- `platform-engineering.md` — 10+ IDP frameworks, developer portals
- `ai-for-devops.md` — 30+ AI tools, MCP servers, agents
- `cost-management-finops.md` — 8+ FinOps tools, savings strategies
- `mlops-llmops-tools.md` — 20+ MLOps/LLMOps tools, lifecycle coverage
- `messaging-streaming.md` — 8+ messaging tools, Kafka alternatives

### Get Started (docs/get-started/)
- `how-to-use-this-list.md` — Navigation guide, progressive disclosure
- `freelance-devops-roadmap.md` — 12-month learning path to $150+/hr

### Careers (docs/careers/)
- `freelancer-profile-analysis.md` — Top profile patterns, rates, strategies

### Reference (docs/reference/)
- `methodology.md` — Research validation process
- `research-review-notes.md` — Quality audit across all research docs
- `how-to-contribute.md` — Contribution guide with quality standards

---

## 🌐 Documentation Site

The project uses **Hugo** with the **Book theme** to build a static documentation site.

- Configuration: `site/hugo.toml`
- Theme: `site/themes/hugo-book` (git submodule)
- Content mounts directly from root `docs/` (no separate copy)
- Deploy URL: `https://adurrr.github.io/awesome-devops-freelance/`

### Building Locally

```bash
cd site
hugo server -D
```

### Deployment

Automatic via GitHub Actions (`.github/workflows/deploy-site.yml`) on pushes to `main` that touch `site/` or `docs/`.
