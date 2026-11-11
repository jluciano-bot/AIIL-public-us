<!-- aiil-logo-header:start -->
<p align="left"><img src="../../website/Blue%20Hexagon%20Temple%20Logo.png" alt="AIIL - Artificial Intelligence Infrastructure Library" height="72"></p>
<!-- aiil-logo-header:end -->

# AIIL AI Problem Management

Version: 1.0  
Status: Active  
Last Updated: 2026-11-01

---

## Purpose

Identify, investigate, and eliminate the root causes of AI incidents and recurring failures, preventing their recurrence and minimizing the overall impact of unavoidable incidents.

---

## Scope

All recurring AI incidents, systemic failures, and known weaknesses identified across AI services, models, agents, prompts, and data pipelines.

---

## Definitions

| Term | Definition |
|---|---|
| Problem | The unknown root cause of one or more AI incidents |
| Known Error | A problem where the root cause and a workaround (or fix) have been identified |
| Root Cause Analysis (RCA) | Structured investigation to identify the underlying cause of a problem |

---

## Problem Sources

Problems may originate from:
- Recurring incidents of the same type
- Trend analysis revealing patterns
- Proactive reviews identifying risks before incidents occur
- Post-incident reviews (PIR)
- External intelligence (model provider advisories, AI security disclosures)

---

## AI Problem Categories

| Category | Description | Examples |
|---|---|---|
| Prompt Design | Systematic prompt failures | Ambiguous instructions, missing constraints, poor examples |
| Model Limitations | Inherent model weaknesses | Knowledge cutoff, reasoning gaps, hallucination patterns |
| Data Quality | Data feeding incorrect context | Stale knowledge bases, inconsistent data sources |
| Integration | Systematic integration failures | API instability, context window exhaustion |
| Governance | Process gaps enabling recurring failures | No change controls, undocumented agents |
| Security | Exploitable weaknesses | Repeated prompt injections, unvalidated outputs |

---

## Process Flow

### Step 1 — Problem Identification

Trigger sources:
- Threshold exceeded (e.g., same incident type >3 times in 30 days)
- Post-Incident Review recommendation
- Proactive review finding
- User feedback trend

### Step 2 — Problem Logging

Record the problem with:
- Date identified
- Related incident records
- Description of the problem pattern
- Assigned Problem Manager
- Priority

### Step 3 — Problem Classification

Classify by:
- Category (Prompt, Model, Data, Integration, Governance, Security)
- Priority (P1–P4 mirroring incident severity)
- Scope (single service vs. multiple services)

### Step 4 — Root Cause Investigation

Apply structured investigation techniques:

**5 Whys Analysis**
Iteratively ask "why" until the root cause is identified.

**AI-Specific Fishbone Analysis**
Examine:
- Prompt design
- Model selection and configuration
- Training data quality
- Context and retrieval mechanisms
- Governance and oversight gaps
- Security controls

**Reproducibility Testing**
Attempt to reproduce the failure in a non-production environment to confirm the root cause hypothesis.

### Step 5 — Known Error Declaration

Once root cause is identified:
- Record as Known Error
- Document workaround if permanent fix is not immediately available
- Publish to Known Error Database (KEDB)
- Notify AI Service Desk to apply workaround to related incidents

### Step 6 — Solution Development

Options:
- Prompt redesign
- Model parameter adjustment
- Model replacement
- Data pipeline remediation
- Process or governance control improvement
- Security control enhancement

### Step 7 — Change Initiation

Raise a Change Request through AI Change Management to implement the solution. Problem Management drives the what; Change Management governs the how.

### Step 8 — Problem Resolution

- Verify solution eliminates root cause
- Confirm related incidents cease to recur
- Update KEDB
- Close Problem Record

### Step 9 — Post-Problem Review

For P1/P2 problems:
- Document lessons learned
- Identify process improvements
- Submit improvement actions to AI Continual Improvement

---

## Known Error Database (KEDB)

The KEDB records all Known Errors and their associated workarounds.

Each KEDB entry contains:
- Known Error ID
- Description
- Affected services
- Root cause summary
- Available workaround
- Status (Open, Fix in Progress, Resolved)
- Related Change Request

---

## Proactive Problem Management

AIIL recommends a proactive review cadence:

| Review Type | Frequency | Inputs |
|---|---|---|
| Incident trend analysis | Monthly | Incident records |
| Model performance review | Quarterly | KPI dashboards |
| Prompt quality audit | Quarterly | User feedback, incident data |
| Agent behavior review | Quarterly | Agent logs, incident records |
| Known error review | Monthly | KEDB |

---

## Roles and Responsibilities

| Role | Responsibility |
|---|---|
| Problem Manager | Own and drive all problem investigations |
| AI Engineer | Technical root cause investigation |
| AI Service Owner | Approve resolution approach |
| AI Operations Manager | Oversee problem process maturity |
| Change Manager | Receive and process change requests from Problem Management |

---

## Key Performance Indicators

| KPI | Target |
|---|---|
| Mean Time to Root Cause (MTTRC) | < 5 business days for P1 |
| Recurring incident rate | < 10% of monthly incidents |
| KEDB completeness | 100% of known errors documented |
| Problems resolved within SLA | > 90% |
| Proactive vs. reactive problem ratio | > 30% proactive |

---

## Outputs

- Problem Record
- Root Cause Analysis Report
- Known Error Database (KEDB) entry
- Change Request (for solution implementation)
- Post-Problem Review Report
- Improvement Actions

---

## Integration with Other AIIL Processes

- **AI Incident Management** — incidents are the primary input to problem management
- **AI Change Management** — solutions are implemented through change management
- **AI Risk Management** — known errors may generate risk entries
- **AI Continual Improvement** — lessons learned feed improvement initiatives
- **AI Knowledge Management** — KEDB is a knowledge management artifact

---

## AIIL Principle

Fixing incidents is not enough. Organizations must systematically investigate and eliminate the root causes of AI failures to achieve sustainable operational reliability.
