# SRE Tools — Extended List

> **Purpose**: Comprehensive comparison of Site Reliability Engineering tools across all categories — SLI/SLO management, incident response, on-call scheduling, chaos engineering, AI SRE, runbook automation, and status pages.

**Last updated**: 2026-05-29

---

## 1. SLI / SLO Management Platforms

| Tool | Description | Pricing | Key Features | Freelance Use |
|---|---|---|---|---|
| **[Nobl9](https://nobl9.com)** | The leading SLO platform; OpenSLO co-creator | $30+/user/mo (Free tier available) | SLO-as-Code (OpenSLO), multi-source SLIs, error budget alerts, SLO dashboards | Design SLO frameworks for clients; integrate OpenSLO into existing observability stacks |
| **[Chronosphere](https://chronosphere.io)** | Observability platform with built-in SLO management | Custom pricing | SLO monitoring, cost-controlled observability, Grafana integration, alert suppression | Enterprise SRE consulting; help clients reduce observability costs while maintaining SLOs |
| **[Squadcast](https://squadcast.com)** | Incident response + SLO monitoring in one platform | $19+/user/mo (SLO in Premium tier $29) | Integrated SLO tracking + incident response, error budget alerts, AI alert grouping | Mid-market SRE teams wanting unified incident + SLO platform |
| **[Google Cloud Monitoring](https://cloud.google.com/monitoring)** | Native SLO management for GCP | Pay-per-use (included in GCP) | Custom SLIs, SLO monitoring, alerting policies, error budget reporting | GCP-native clients; simplest SLO setup for Google Cloud shops |
| **[Datadog SLOs](https://www.datadoghq.com)** | SLO tracking within Datadog observability | Included in Pro+ plans | Multi-source SLIs, error budget widgets, SLO alerts, correction windows | Clients already on Datadog; add SLO layer to existing monitoring |

**Comparison**: Nobl9 is the most SLO-specific (SLO-first platform). Chronosphere excels for cost-conscious enterprises. Squadcast is best for mid-market wanting incident + SLO in one.

---

## 2. Incident Management Platforms

| Tool | Description | Pricing | Key Features | Freelance Use |
|---|---|---|---|---|
| **[PagerDuty](https://pagerduty.com)** | Enterprise incident response standard | $21+/user/mo | On-call scheduling, escalation policies, 700+ integrations, AIOps (PagerDuty AI) | Enterprise deployments; Opsgenie migrations; complex on-call configurations |
| **[incident.io](https://incident.io)** | Slack-native incident coordination | $15+/user/mo | Automated Slack channels, timeline capture, AI postmortems, status pages | Clients with Slack-native workflows; modern incident response setup |
| **[Rootly](https://rootly.com)** | Automation-heavy incident management | $15+/user/mo | AI incident summarization, 300+ integrations, retrospectives, severity-based workflows | SRE teams wanting deep automation; platform teams |
| **[Squadcast](https://squadcast.com)** | SRE-focused incident response | $19+/user/mo | SLO-integrated incident response, AI alert grouping, on-call schedules | Mid-market SRE teams wanting all-in-one (incident + SLO + on-call) |
| **[FireHydrant](https://firehydrant.com)** | Incident management + runbook automation | $15+/user/mo | Runbook automation, service catalog, incident timelines, Slack integration | Clients transitioning from Opsgenie; runbook-first approach |
| **[xMatters](https://xmatters.com)** | Enterprise incident communication | Custom pricing | On-call scheduling, intelligent alerting, ITSM integrations, collaboration tools | Large enterprises with complex on-call hierarchies |

**2026 Market Shift**: Opsgenie (Atlassian) stopped new sales June 2025, EOL April 2027 → massive migration opportunity. Grafana OnCall OSS archived March 2026. FireHydrant acquired by Freshworks Jan 2026.

---

## 3. Observability & Monitoring

See also → [full Observability & Monitoring comparison](observability-monitoring.md)

| Tool | Description | Deployment | Key SRE Features | Freelance Use |
|---|---|---|---|---|
| **[Datadog](https://datadoghq.com)** | Full-stack observability | SaaS | AI-driven alerts (Watchdog), SLO dashboards, Bits AI assistant, APM | Comprehensive SRE monitoring; premium pricing justified for enterprise clients |
| **[Grafana + Prometheus](https://grafana.com)** | Open-source monitoring stack | OSS / Grafana Cloud | PromQL for SLO calculations, Grafana SLO dashboards, alerting, Loki for logs | Cost-conscious clients; SLO dashboards built on open source |
| **[New Relic](https://newrelic.com)** | Observability platform | SaaS | AI-powered root cause analysis, SLO monitoring, browser monitoring | Application-focused SRE; front-end reliability tracking |
| **[Chronosphere](https://chronosphere.io)** | Metrics-focused observability | SaaS | Cost-controlled metrics, SLO management, cardinality management | Enterprises with large-scale metrics and observability cost challenges |
| **[Honeycomb](https://honeycomb.io)** | Observability for debugging | SaaS | High-cardinality querying, bubble-up for root cause, SRE-specific queries | Debugging complex distributed systems; production debugging |
| **[Checkly](https://checklyhq.com)** | Synthetic monitoring for SREs | SaaS | Playwright-based browser checks, API monitoring, Terraform provider, status pages | SREs practicing "monitoring-as-code"; CI/CD-integrated checks |

**Note**: The SRE Report 2026 found that **55% of teams spend a fair amount or a lot of time integrating or connecting tools** — a significant freelance opportunity for tool consolidation and platform integration.

---

## 4. Chaos Engineering Tools

| Tool | Description | Deployment | Key Features | Freelance Use |
|---|---|---|---|---|
| **[LitmusChaos](https://litmuschaos.io)** | CNCF chaos engineering platform | OSS / SaaS | K8s-native, CI/CD integration, custom chaos experiments, detailed metrics | Kubernetes-focused clients; integrating chaos into existing pipelines |
| **[Chaos Mesh](https://chaos-mesh.org)** | CNCF chaos engineering for K8s | OSS | DNS chaos, network partition, pod-kill, stress injection, web UI | Lightweight chaos experiments on K8s; simpler setup than Litmus |
| **[Gremlin](https://gremlin.com)** | SaaS chaos engineering platform | SaaS | Host, container, and K8s attacks; safe experiments; GameDay facilitation | Clients wanting managed chaos engineering without OSS overhead |
| **[ChaosBlade](https://chaosblade.io)** | Alibaba's chaos engineering tool | OSS | Multi-protocol (K8s, Docker, Java), rich failure scenarios | Multi-environment chaos experiments; Alibaba ecosystem clients |
| **[AWS Fault Injection Simulator](https://aws.amazon.com/fis)** | AWS-native chaos testing | AWS | Integrated with AWS services, pre-built templates, safe by default | AWS-native clients; simplest option for AWS workloads |

**The SRE Report 2026**: Only **17%** run chaos/resilience experiments in production regularly — massive room for growth. Freelance opportunity to establish chaos engineering programs from scratch.

---

## 5. AI SRE Tools (Emerging)

| Tool | Description | Key Features | Best For |
|---|---|---|---|
| **[Datadog Bits AI](https://www.datadoghq.com/product/bits-ai)** | AI assistant for Datadog | Natural language query, root cause analysis, anomaly investigation | Existing Datadog customers; comprehensive telemetry + AI |
| **[incident.io AI SRE](https://incident.io/ai-sre)** | AI incident response assistant | Alert triage, code change correlation, fix drafting, postmortem generation | Slack-native incident workflows; coordination-first teams |
| **[Rootly AI](https://rootly.com)** | AI for incident management | Incident summarization, severity classification, action item extraction | Automation-heavy SRE teams; multi-tool workflows |
| **[Better Stack AI](https://betterstack.com)** | All-in-one observability + AI | AI SRE assistant, incident management, status pages, uptime monitoring | Small to mid-market teams wanting affordable all-in-one |
| **[Metoro](https://metoro.io)** | Kubernetes-native AI RCA | Deployment-aware RCA, K8s runtime context, fix generation | K8s-heavy environments; deep runtime context |
| **[HolmesGPT](https://github.com/robusta-dev/holmesgpt)** | Open-source AI incident investigator | Multi-source investigation, K8s integration, CNCF Sandbox | Teams wanting OSS AI SRE without vendor lock-in |

> See also: [AI for DevOps extended list](./ai-for-devops.md) for broader AI + operations tools.

---

## 6. Runbook Automation & Operations

| Tool | Description | Pricing | Key Features | Freelance Use |
|---|---|---|---|---|
| **[Rundeck](https://rundeck.com)** | Self-service operations automation | OSS / $1+/node/mo | Job scheduling, runbook automation, RBAC, PagerDuty integration | Automating incident response runbooks; setting up self-service ops for platform teams |
| **[PagerDuty Operations Cloud](https://pagerduty.com)** | Unified incident + automation | Enterprise | Automated remediation, runbook workflows, AI-driven operations | Enterprise clients consolidating incident + runbook tooling |
| **[FireHydrant Runbooks](https://firehydrant.com)** | Incident-specific runbooks | Included in FireHydrant | Step-by-step incident workflows, automated timelines, service catalog linking | Teams adopting structured incident response with automated runbooks |
| **[Checkly](https://checklyhq.com)** | Monitoring-as-code + runbooks | $25+/user/mo | Playwright-based checks, Terraform-managed, auto-remediation scripts | SREs who codify everything; CI/CD-native runbooks |

---

## 7. Status Pages

| Tool | Description | Pricing | Key Features | Freelance Use |
|---|---|---|---|---|
| **[Atlassian Statuspage](https://atlassian.com/software/statuspage)** | Market-leading status pages | Free / $59+/mo | Custom domains, subscriber notifications, API, component status | Client-facing status pages; incident communication |
| **[incident.io Status Pages](https://incident.io)** | Status pages built into incident response | Included in incident.io | Automatic incident→status page sync, subscriber management | Teams already on incident.io; unified incident + status page |
| **[Better Stack Statuspage](https://betterstack.com/statuspage)** | Affordable status pages | Free / $24+/mo | Uptime monitoring, status pages, public API, team collaboration | Budget-conscious clients; simple status page needs |
| **[Checkly Status Pages](https://checklyhq.com)** | Monitoring-native status pages | Included in Checkly | Auto-generated from checks, custom branding, subscriber management | Teams using Checkly for monitoring; zero-config status pages |

---

## 8. Comparison: Key Purchase Criteria

| Category | Must-Have | Nice-to-Have | Avoid |
|---|---|---|---|
| **Incident Management** | Slack integration, on-call scheduling, escalation policies | AI summarization, postmortem automation, status page sync | Rigid ITSM workflows (SRE teams moved away from this) |
| **SLO Platforms** | Multi-source SLIs, error budget alerts, SLO dashboards | SLO-as-Code (OpenSLO), GitOps integration, cost controls | Platforms requiring agent installation for SLIs |
| **Chaos Engineering** | K8s support, safe guardrails, experiment rollback | CI/CD integration, GameDay templates, detailed reports | Tools that only work in non-production (defeats purpose) |
| **Observability** | OpenTelemetry support, PromQL, high-cardinality | eBPF, continuous profiling, AI correlation | Vendor lock-in telemetry formats |
| **AI SRE** | Natural language query, alert context, tool integration | Root cause analysis, auto-remediation, postmortem generation | Black-box AI (need explainability for postmortems) |

---

## 9. SRE Tool Stack by Team Size

| Team Size | Recommended Stack | Monthly Cost (approx) |
|---|---|---|
| **Startup (<10 devs)** | Grafana Cloud (free tier) + Better Stack ($0-24/mo) + LitmusChaos (OSS) | $0–50/mo |
| **Mid-market (10–50 devs)** | Datadog/New Relic + incident.io or Squadcast ($15-29/user/mo) + Nobl9 ($30/user/mo) + Gremlin ($500-2000/mo) | $1,000–5,000/mo |
| **Enterprise (50+ devs)** | Chronosphere + PagerDuty ($50+/user/mo Enterprise) + Nobl9 + Gremlin Enterprise | $5,000–50,000+/mo |

**Freelance strategy**: Help clients right-size their SRE stack. Most mid-market teams are **over-tooled** (55% spend excessive time on tool integration) and can consolidate.

---

## 10. Learning Resources for SRE

| Resource | Type | Cost | Best For |
|---|---|---|---|
| Google SRE Book | Book (free online) | Free | Foundational SRE knowledge |
| Google SRE Workbook | Book (free online) | Free | Hands-on SRE implementation |
| Catchpoint SRE Report 2026 | Report | Free | 2026 industry benchmarks and trends |
| OpenSLO Specification | Specification | Free | SLO-as-Code implementation |
| Chaos Engineering (O'Reilly) | Book | ~$40 | Chaos engineering program design |
| Cloud Native SRE (O'Reilly) | Book | ~$50 | Cloud-native reliability practices |
| SRECon / USENIX | Conference | $500–2000 | Networking + cutting-edge SRE |

---

*This list is maintained as part of the Awesome DevOps Freelance project. Contributions welcome via PR.*
