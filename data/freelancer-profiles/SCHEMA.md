# Freelancer Profile Schema

Every profile file under `data/freelancer-profiles/real/` MUST follow this schema for consistency and machine-readability.

## File Naming

```
<firstname>-<lastname>-<platform>.md
```

Examples: `antonio-diaz-malt.md`, `bret-fisher.md`, `daniel-c-upwork.md`

Use lowercase, hyphens between name segments and platform suffix. If only personal brand (no platform), omit the platform suffix: `bret-fisher.md`.

## Required Fields

These fields MUST appear at the top of every profile file in the YAML-like header format:

```
**Role**: <job title>
**Location**: <city, country>
```

### Field Reference

| Field | Format | Example | Required |
|-------|--------|---------|----------|
| `**Role**` | Job title | `Platform/DevOps Engineer` | ✅ |
| `**Location**` | City, Country | `Córdoba, Spain` | ✅ |
| `**Platform**` | Platform or "Personal Brand" | `Malt.com`, `Upwork`, `Personal Brand` | ✅ |
| `**Trust Rating**` | `verified` / `likely` / `limited` | `verified` | ✅ |
| `**Rate**` | Amount/period | `€400/day`, `$100/hr`, `Custom consulting (not public)` | ✅ |
| `**Experience**` | Years | `3–7 years`, `20 years` | ✅ |

## Optional Fields

| Field | Format | Example |
|-------|--------|---------|
| `**Profile URL**` | Full URL | `https://bretfisher.com` |
| `**Blog**` | Full URL | `https://bretfisher.com/blog` |
| `**Response time**` | Duration | `~1 hour` |
| `**Status**` | Verification detail | `✅ verified (Malt.com profile with verifiable work history)` |
| `**Languages**` | Languages | `English, Spanish` |

## Section Structure

After the header fields, organize the profile into these sections (in order):

### 1. Overview (optional)
Brief professional summary. 1-3 paragraphs max.

### 2. Skills (recommended)
Categorized skill list. Use `###` subsections for categories:

```markdown
## Skills

### Cloud Platforms
- AWS, Azure, GCP

### Containers & Orchestration
- Kubernetes, Docker, Helm
```

### 3. Experience (optional)
Work history with dates. Each entry:

```markdown
### Company Name — Job Title
*Month Year – Month Year | Location*
- Responsibility or achievement
```

### 4. Key Highlights (optional)
Bullet list of notable achievements, certifications, publications.

### 5. Trust Assessment (required)
A table documenting verification criteria:

```markdown
## Trust Assessment

| Criterion | Assessment |
|-----------|------------|
| Platform verification | ✅ Malt.com profile with detailed experience timeline |
| Rate transparency | ✅ €400/day listed |
| Work history | ✅ Detailed, verifiable positions |
| Identity | ✅ Full name, location |
| Skills breadth | ✅ Multi-cloud, IaC, observability |

**Overall**: ✅ **Verified** — Description of why this rating.
```

### 6. Sources (required)
List of URLs where the profile data was obtained:

```markdown
## Sources
- Malt.com profile: https://malt.com/profile/example
```

## Trust Rating Definitions

| Rating | Meaning | Requirements |
|--------|---------|--------------|
| `verified` | High confidence in identity, skills, and location | Multi-source verification, detailed work history, public profiles |
| `likely` | Reasonable confidence, some data points | Platform profile with reviews, portfolio samples, or GitHub presence |
| `limited` | Low confidence, sparse data | Single source, minimal verification possible |

## Template

```markdown
# Full Name

**Role**: Job Title
**Location**: City, Country
**Platform**: Platform Name
**Rate**: €XXX/day
**Experience**: X years
**Response time**: ~X hours

## Overview

Brief professional summary.

## Skills

### Category
- Skill 1
- Skill 2

## Experience

### Company — Title
*Month Year – Month Year | Location*
- Achievement or responsibility

## Trust Assessment

| Criterion | Assessment |
|-----------|------------|
| Criterion | ✅ Assessment |

**Overall**: ✅ **Rating** — Justification.

## Sources
- Platform profile: URL
```

## Validation

- All sources must be real, publicly accessible URLs
- Rate formats: `€400/day`, `$100/hr`, `EUR 500/day`, `Custom (not public)`
- Dates in `YYYY-MM-DD` format for "Last updated" headers
- Trust rating must be one of: `verified`, `likely`, `limited`
