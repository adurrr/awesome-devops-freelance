# Infrastructure as Code Tools → Extended List

> **Full comparison of IaC tools for DevOps freelancers.**

---

## Comparison Matrix

| Tool | Language | License | Stars | IaC Type | Multi-Cloud | Learning Curve | Freelance Demand |
|---|---|---|---|---|---|---|---|
| **Terraform** | HCL | BSL | 43k+ | Provisioning | ✅ | Medium | 🔥🔥🔥🔥🔥 |
| **OpenTofu** | HCL | MPL | 22k+ | Provisioning | ✅ | Medium | 🔥🔥🔥🔥 Growing |
| **Pulumi** | Python/TS/Go/C# | Apache 2.0 | 22k+ | Provisioning | ✅ | Medium-High | 🔥🔥🔥 Growing |
| **Crossplane** | K8s CRDs (YAML) | Apache 2.0 | 10k+ | Control plane | ✅ | High | 🔥🔥 Niche premium |
| **Ansible** | YAML | GPL | 63k+ | Config mgmt | ✅ | Low-Medium | 🔥🔥🔥🔥 Steady |
| **CloudFormation** | JSON/YAML | AWS | - | Provisioning | ❌ (AWS) | Medium | 🔥🔥 AWS-only |
| **Puppet** | DSL | Apache 2.0 | 8k+ | Config mgmt | ✅ | High | 🔥 Legacy |
| **Chef** | Ruby DSL | Apache 2.0 | 8k+ | Config mgmt | ✅ | High | 🔥 Legacy |

## Key Tools Detailed

### Terraform
- **Freelance use case**: 90% of infrastructure gigs need Terraform
- **Rate impact**: Baseline IaC skill
- **Best for**: Multi-cloud provisioning, state management
- **Alternatives**: OpenTofu (open-source fork)

### OpenTofu
- **Why it matters**: Linux Foundation-backed Terraform fork after BSL license change
- **Freelance use case**: Clients avoiding Terraform BSL license
- **Adoption**: Growing rapidly (22k GitHub stars)

### Pulumi
- **Why it matters**: IaC in real programming languages
- **Freelance use case**: Teams that prefer Python/TypeScript over HCL
- **Premium**: Niche skill commands higher rate

### Crossplane
- **Why it matters**: K8s-native IaC (CNCF graduated Oct 2025)
- **Freelance use case**: Platform engineering, K8s-centric organizations
- **Premium**: +30-40% over Terraform roles

## Freelance Project Ideas
1. Multi-cloud infrastructure with Terraform workspaces (dev/staging/prod)
2. Migration from CloudFormation → Terraform
3. Crossplane control plane for platform engineering
4. Ansible playbooks for configuration management
5. OpenTofu migration from Terraform
