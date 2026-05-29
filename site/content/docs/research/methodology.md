---
title: "Research Methodology"
weight: 10
---

# Research Methodology

> **Purpose**: Documents how research is conducted, validated, and maintained. Critical for transparency and anti-hallucination.

---

**Last updated**: 2026-05-26


### Tier 1: Primary Sources (Highest Trust)
- Official documentation (project docs, READMEs, official websites)
- CNCF landscape ([landscape.cncf.io](https://landscape.cncf.io/))
- GitHub repository data (stars, forks, activity)
- Published academic papers (arXiv, ACM, IEEE)
- Industry reports (Perforce, CNCF, Gartner, Forrester)

### Tier 2: Secondary Sources (Medium Trust)
- Technical blogs from recognized experts
- Freelance platform profiles (Toptal, Upwork, Arc.dev)
- Community surveys (CNCF annual survey, Stack Overflow)
- Vendor-published case studies

### Tier 3: Tertiary Sources (Lower Trust, Cross-Referenced)
- Aggregator posts and listicles
- Social media discussions
- General articles (unless author has established expertise)
- AI-generated summaries (always verified against primary sources)

---

## 2. Validation Process

### Tool Validation
1. Check GitHub stars and last commit date
2. Verify CNCF status (if applicable)
3. Check for "deprecated" or "archived" status
4. Cross-reference pricing if available
5. Verify tool exists and works as described

### Market Data Validation
1. Source must be explicitly cited (not "experts say")
2. Cross-reference with 2+ sources when possible
3. If only 1 source exists, mark as "according to [source]"
4. If contradictory data exists, present both with sources

### Academic Validation
1. Trace every claim to DOI, arXiv ID, or ISBN
2. Verify the paper exists in the claimed venue
3. Confirm cited finding is accurately represented
4. Note if findings are from SLR vs single study

### Rate/Pricing Validation
1. Cross-reference across 3+ platforms
2. Note date of data collection
3. Distinguish between posted rates and realized rates
4. Flag outliers explicitly

---

## 3. Uncertainty Language

| Phrase | Meaning |
|---|---|
| "According to [source]" | Directly sourced |
| "Industry consensus" | Widely agreed, no single source |
| "Suggests" | Indicates but not conclusively proven |
| "Sparse evidence" | Limited backing |
| "Emerging" | Early stage, may change |
| "~[number]" | Approximate |
| "[range] estimated" | Reasonable estimate |

---

## 4. Update Cycle

- **Monthly**: Link checking, status updates
- **Quarterly**: Major review of each research doc
- **Annually**: Complete re-evaluation of all paradigms

---

## 5. AI Usage Disclosure

AI is used in this project as a productivity tool for:
- Draft generation and structuring
- Cross-referencing claims across sources
- Summarizing research findings
- Identifying potential new sources

AI is NOT used for:
- Inventing tools, companies, or products
- Creating fake citations or references
- Fabricating metrics or statistics
- Generating content without human verification

All AI-assisted content is verified against primary sources before inclusion.

---

## 6. Correction Process

1. Error reported via issue, PR, or direct contact
2. Error assessed against primary sources
3. If confirmed: correction added, original marked with note
4. Change logged in CHANGELOG.md
5. If AI hallucination: flagged and root cause analyzed

---

## 7. Sources Integrity

- All URLs verified at time of inclusion
- Broken URLs tracked monthly via automated check
- Wayback Machine links used when original URL is unstable
- PDF and page captures kept for critical sources
