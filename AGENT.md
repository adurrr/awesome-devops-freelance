# AGENT.md — AI Agent Instructions

> **Purpose**: Instructions for AI agents (including this one) working on the awesome-devops-freelance project. Ensures consistency, quality, and anti-hallucination compliance.

---

## 🎯 Project Context

**Name**: awesome-devops-freelance  
**Type**: Curated awesome list + research documentation  
**License**: AGPL-3.0  
**Audience**: DevOps freelancers, platform engineers, SRE consultants  
**Scope**: All Ops paradigms (DevOps, DevSecOps, DataOps, MLOps, AIOps, FinOps, LLMOps, Platform Engineering, SRE, GitOps)

---

## 📝 Content Standards

### When Adding a Tool

**Required fields** (every tool entry must have):
1. **Name + URL** — Link to official site or GitHub repo
2. **Badges** — At minimum: GitHub stars (if applicable), license, CNCF status (if applicable)
3. **One-line description** — What it does
4. **Freelance use case** — Why it matters for freelancers (this is the differentiator)

**Badge format** (use shields.io):
```markdown
![GitHub stars](https://img.shields.io/github/stars/OWNER/REPO?style=flat-square)
![License](https://img.shields.io/badge/license-Apache%202.0-green)
![CNCF](https://img.shields.io/badge/CNCF-Graduated-blue)
![CNCF](https://img.shields.io/badge/CNCF-Incubating-orange)
![CNCF](https://img.shields.io/badge/CNCF-Sandbox-yellow)
```

**Entry format**:
```markdown
- **[Tool Name](URL)** ![badges] — One-line description. **Freelance use**: Why it matters.
```

### When Writing Research Docs

**Structure**:
1. Definition and scope
2. Key trends (with year context)
3. Tool landscape (lists with badges, not tables)
4. Freelance opportunities (rate ranges)
5. Academic references (with DOI/arXiv ID)
6. Sources (all claims traced)

**Anti-hallucination rules**:
- Every factual claim must have a source
- Use uncertainty language for estimates ("~25%", "according to [source]")
- Never invent tools, companies, or metrics
- Cross-reference market data with 2+ sources
- If only 1 source exists, explicitly state it

### When Updating Existing Content

**Checklist**:
- [ ] Verify all URLs are still working
- [ ] Check GitHub stars are current
- [ ] Confirm CNCF status hasn't changed
- [ ] Update "Last updated" date in document
- [ ] Check if tool has been deprecated
- [ ] Verify freelance rate data is still current

---

## 🔍 Research Protocol

### Finding New Tools
1. Search GitHub trending for relevant keywords
2. Check CNCF landscape updates
3. Review Hacker News / Reddit / Twitter discussions
4. Verify tool meets inclusion criteria (500+ stars OR CNCF OR commercial proven)

### Validating Claims
1. Primary source first (official docs, GitHub, CNCF)
2. Cross-reference with 2+ sources for market data
3. Academic claims need DOI or arXiv ID
4. Rate data needs 3+ platform references

### What NOT to do
- ❌ Invent tools or companies
- ❌ Create fake GitHub star counts
- ❌ Fabricate academic citations
- ❌ Copy content without attribution
- ❌ Add tools you haven't verified exist
- ❌ Claim CNCF status without checking landscape.cncf.io

---

## 🏗 Directory Structure

```
awesome-devops-freelance/
├── README.md                    ← Main curated list (lists + badges, NOT tables for tools)
├── docs/
│   ├── research/                ← Deep dives (standalone documents)
│   ├── extended-lists/          ← Detailed tool references
│   └── guides/                  ← User-facing guides
├── research/
│   └── methodology.md           ← Research process documentation
└── .github/                     ← Templates and workflows
```

**Rules**:
- README uses **lists with badges** for tools; tables only for comparisons/summaries
- Research docs use **lists with badges** for tools; tables for paradigm comparisons
- Extended lists can use tables for detailed comparisons
- All documents must include "Last updated: YYYY-MM-DD"

---

## 🎨 Style Guide

### Markdown Formatting
- Use `##` for main sections, `###` for subsections
- Use `-` for unordered lists (not `*`)
- Use `1.` for ordered lists
- Code blocks with language tags: ```bash, ```yaml, ```json
- Inline code for tool names: `kubectl`, `terraform`

### Tone
- Direct and actionable ("Use this for..." not "One might consider...")
- Freelancer-first (every entry answers "why for freelancers")
- Evidence-based (sources cited, not opinion)
- Current (2026 context, not historical unless specified)

### Emojis
- Use sparingly for section headers only
- Allowed: 🏆, 📋, 🔬, 💼, 📚, 🤝, 📄, 🌟, ✅, ❌, 🔄, 🆕
- Avoid in body text

---

## 🔄 Maintenance Tasks

### Monthly
- Run link checker
- Review open issues and PRs
- Check for new CNCF project graduations
- Update tool statuses

### Quarterly
- Refresh research documents with new trends
- Update freelancer rate data
- Review and prune deprecated tools
- Add new tools from community suggestions

### Annually
- Complete paradigm re-evaluation
- Refresh top 50 freelancer analysis
- Update platform comparisons
- Review and update roadmap

---

## 🆘 When Stuck

**If you can't verify a claim**:
- Mark it as "unverified" or "according to [single source]"
- Do not present it as fact
- Add a TODO comment for human review

**If you find contradictory information**:
- Present both sides with sources
- Note the discrepancy explicitly
- Let the community or maintainer resolve it

**If a tool doesn't meet inclusion criteria**:
- Do not add it to the main list
- You may mention it in a research doc with context
- Suggest it in an issue for community discussion

---

## 📋 Pre-Submission Checklist

Before generating or modifying any file, verify:

- [ ] All tool URLs are real and working
- [ ] GitHub star counts are accurate (check live)
- [ ] CNCF status is verified on landscape.cncf.io
- [ ] License information is correct
- [ ] Freelance use case is specific and actionable
- [ ] No AI hallucinations (invented tools, fake citations)
- [ ] Format follows style guide (lists + badges, not tables for tools)
- [ ] "Last updated" date is current
- [ ] Sources are cited for all factual claims

---

## 🧠 Context for AI Agents

This project is NOT just a list of tools. It is:
1. A **curated resource** for freelancers to make money
2. A **research document** grounded in academic literature
3. A **career guide** based on real freelancer data
4. A **living document** that requires ongoing maintenance

Every decision should prioritize:
1. **Accuracy** over comprehensiveness
2. **Freelancer value** over tool popularity
3. **Verifiability** over convenience
4. **Long-term maintainability** over short-term completeness

When in doubt, ask the human maintainer. Do not guess.
