# 🤝 How to Contribute

> A detailed guide for contributing to Awesome DevOps Freelance → beyond the quick start in [`CONTRIBUTING.md`](https://github.com/adurrr/awesome-devops-freelance/blob/main/CONTRIBUTING.md).

**Last updated**: 2026-05-26

---

## Contribution Philosophy

This project aims to be the **most comprehensive curated DevOps freelance resource**. Every contribution should:

- **Add real value** for DevOps freelancers
- **Be verified** against primary sources
- **Follow the format** of existing content
- **Be current** (published or updated within the last 24 months)

---

## 🛠 Adding a Tool

### Eligibility Criteria

A tool qualifies if it meets **at least one** of:

- **500+ GitHub stars** (verified at time of submission)
- **CNCF project** (any stage: sandbox, incubating, or graduated)
- **Commercially proven** (significant enterprise adoption → provide evidence)

AND is **relevant to DevOps freelancers** (used in client work, proposals, or operations).

### Where to Add It

| Tool Type | Where to Add |
|---|---|
| New tool in existing category | The corresponding extended list in `docs/extended-lists/` |
| New category entirely | Propose first via issue, then add to README + new extended list |
| Correction or update | PR directly against the affected document |

### Format for Extended Lists

Each tool entry should follow this structure:

```markdown
### [Tool Name](https://tool-url.com)
![GitHub stars](https://img.shields.io/github/stars/owner/repo?style=flat-square)
![License](https://img.shields.io/badge/license-LicenseName-blue)
→ One-line description of what it does.
**Freelance use**: Why this matters for freelancers (1-2 sentences).
```

### Requirements for New Entries

- [ ] Tool meets eligibility criteria
- [ ] GitHub stars or license badge included (for open-source tools)
- [ ] Description is factual, not marketing
- [ ] "Freelance use" explains concrete value (not generic "it's useful")
- [ ] No affiliate links without explicit disclosure
- [ ] Pricing is verified and includes date of verification
- [ ] Cross-link to related tools or docs where relevant

---

## 📝 Updating a Resource

### Fixing Outdated Information

| Change | Action |
|---|---|
| Broken URL | Open PR with corrected URL |
| Outdated pricing | Open issue or PR with new data + source |
| Tool status change | PR updating the status (e.g., CNCF graduated) |
| Rate data refresh | Issue with new data from 3+ sources |

### Updating Documentation

When making substantive updates:

1. Update the **Last updated** date at the top of the document
2. Add a brief summary of changes in the PR description
3. If removing content, explain why (deprecated, irrelevant, incorrect)
4. If adding content, ensure it follows existing format and style

---

## 🆕 Suggesting a New Category

The DevOps landscape evolves quickly. To suggest a new category:

1. **Open an issue** with the `new-category` label
2. Include:
   - Category name and description
   - 3+ tools that would belong in this category
   - Why it matters for DevOps freelancers
   - Supporting market data or trends
3. **Wait for community discussion** before implementing

Categories are accepted based on:
- **Freelance demand** → Is there paid work in this area?
- **Tool ecosystem maturity** → Are there enough tools to warrant a category?
- **Community interest** → Are others asking for this?

---

## 🔬 Academic References

Help ground the project in research by contributing academic references:

1. Open a PR against `docs/research/academic-references.md`
2. Include for each reference:
   - Full citation (APA or IEEE format)
   - DOI or arXiv ID
   - 2-3 sentence summary of findings
   - Which paradigm(s) it relates to
   - Whether it's open access or paywalled

**Preferred sources**: ACM, IEEE, arXiv, MDPI, Springer, Elsevier → published within 2017-2026.

---

## 💼 Freelancer Insights

### Sharing Rate Data

If you have real-world DevOps freelance rate data:

1. Open an issue with the `data` label
2. Include: platform, specialization, experience level, rate range, geographic region
3. Anonymize client-specific information
4. Specify data collection date and method

### Profile Pattern Suggestions

Noticed a pattern we missed in the top-50 analysis? Open an issue or PR with:
- The pattern (headline formula, portfolio element, engagement tactic)
- Supporting evidence (examples without personal info)
- Why you think it converts

---

## ✅ Quality Checklist

Before submitting any contribution, verify:

- [ ] **No AI-generated content** → all claims are traceable to real sources
- [ ] **No duplicate entries** → check existing content first
- [ ] **All URLs work** → test every link
- [ ] **Formatting matches** → consistent with surrounding content
- [ ] **Sources included** → for all factual claims, market data, and pricing
- [ ] **Freelance value stated** → every entry answers "why this matters"
- [ ] **No promotional language** → factual, not marketing

---

## 🔄 Contribution Workflow

```
1. Fork the repository
2. Create a feature branch (git checkout -b add-tool-name)
3. Make your changes
4. Run through the quality checklist (above)
5. Commit with clear message
6. Push to your fork
7. Open a Pull Request
```

**PR titles** should follow: `[Type] Brief description of change`
Examples:
- `[Tool] Add Karpenter to IaC extended list`
- `[Update] Fix broken link in devsecops research doc`
- `[Category] Propose Data Streaming as new category`

---

## 📋 PR Review Process

1. **Automated checks** run (link validation, format verification)
2. **Maintainer review** within 5 business days
3. **Community feedback** period (minimum 48 hours for substantive changes)
4. **Merge** once approved and all checks pass

---

## ❓ Questions?

Open an issue with the `question` label. For urgent matters, ping a maintainer on the PR.

See also: [`CONTRIBUTING.md`](https://github.com/adurrr/awesome-devops-freelance/blob/main/CONTRIBUTING.md) for the quick-reference version.
