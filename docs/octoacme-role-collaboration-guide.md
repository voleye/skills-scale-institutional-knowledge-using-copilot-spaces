# OctoAcme Role Collaboration Guide

This document provides a lightweight responsibility matrix and handoff checklist to help teams understand who is accountable, responsible, consulted, and informed at each stage of a project. It supplements the [Roles and Personas](./octoacme-roles-and-personas.md) document.

---

## RACI Matrix

**Legend**
- **R** — Responsible (does the work)
- **A** — Accountable (final sign-off / owns outcome)
- **C** — Consulted (provides input before a decision)
- **I** — Informed (kept up to date)

| Activity | Project Manager | Product Manager | Developer | Scrum Master | UX Designer / Researcher | Data Analyst | Business Stakeholder | Release Manager |
|---|---|---|---|---|---|---|---|---|
| Define project goals & success metrics | C | A | I | I | C | C | A | I |
| Prioritize backlog | C | A | C | C | C | C | I | I |
| Sprint / iteration planning | A | C | R | R | C | I | I | I |
| Feature design & prototyping | I | C | C | I | A | I | I | I |
| Implementation & code review | I | I | A | I | C | I | I | I |
| QA / acceptance testing | C | A | R | I | C | I | I | C |
| Risk identification & mitigation | A | C | C | C | I | C | C | I |
| Stakeholder status updates | A | C | I | I | I | I | I | I |
| Analytics instrumentation | I | C | R | I | I | A | I | I |
| User research & usability testing | I | C | I | I | A | C | I | I |
| Release readiness check | C | C | C | C | I | I | I | A |
| Deployment execution | I | I | R | I | I | I | I | A |
| Post-release monitoring | C | C | R | I | I | A | I | R |
| Retrospective facilitation | C | I | R | A | I | I | I | C |

---

## Key Handoff Checklist

Use this checklist at critical project transitions to reduce ambiguity and missed context.

### Discovery → Planning
- [ ] Problem statement and success metrics agreed by Product Manager and Business Stakeholder
- [ ] Initial user research findings shared by UX Designer / Researcher with Product Manager
- [ ] Data Analyst consulted on measurable KPIs
- [ ] Project Manager has captured stakeholders, risks, and timeline in the Project Charter

### Planning → Execution
- [ ] Backlog prioritized and sized by Product Manager and Developers
- [ ] Acceptance criteria written for each backlog item
- [ ] Definition of Done agreed by the full team
- [ ] Sprint goals set and communicated by Product Manager and Scrum Master
- [ ] Design specs or wireframes reviewed and approved by Product Manager and Developers

### Execution → Release
- [ ] All acceptance criteria met and PRs merged
- [ ] QA sign-off obtained
- [ ] Release notes drafted and reviewed
- [ ] Rollback plan documented by Release Manager
- [ ] Stakeholders briefed by Project Manager and Release Manager
- [ ] Deployment window confirmed with Operations / Release Manager

### Release → Retrospective
- [ ] Post-deploy smoke tests completed by Release Manager and Developers
- [ ] Incidents or anomalies triaged and documented
- [ ] Success metrics measured by Data Analyst and shared with Product Manager
- [ ] Retrospective scheduled and facilitated by Scrum Master
- [ ] Action items captured and assigned to owners

---

## Cross-Role Communication Summary

| From \ To | Project Manager | Product Manager | Developer | Scrum Master | UX Designer | Data Analyst | Business Stakeholder | Release Manager |
|---|---|---|---|---|---|---|---|---|
| **Project Manager** | — | Weekly sync | Status updates | Blocker escalation | FYI on timeline | Metrics requests | Status reports | Release coordination |
| **Product Manager** | Scope changes | — | Feature specs | Backlog health | Research requests | KPI alignment | Roadmap briefings | Release sign-off |
| **Developer** | Risk flags | PR / demo | — | Blocker reports | Design Q&A | Instrumentation | — | Deployment readiness |
| **Scrum Master** | Process feedback | Backlog concerns | Ceremony facilitation | — | — | — | — | Retrospective findings |
| **UX Designer** | Timeline impacts | Design reviews | Spec walkthroughs | — | — | Quantitative data | Research insights | — |
| **Data Analyst** | Metric summaries | Insight reports | Instrumentation specs | — | Qual/quant synthesis | — | Impact dashboards | Post-release data |
| **Business Stakeholder** | Priority changes | Strategic guidance | — | — | — | ROI feedback | — | Go/no-go decisions |
| **Release Manager** | Release readiness | Release notes | Deployment checklist | Process feedback | — | — | Release announcements | — |

---

## Guidance Notes

- **Avoid RACI gaps**: Every activity should have exactly one Accountable owner. If a cell is blank and a question arises, escalate to the Project Manager.
- **Handoffs require documentation**: Always capture decisions, outstanding risks, and open questions in the project board or shared notes before handing off.
- **Consult early**: Loop in Consulted roles before finalizing decisions—late consultation is a leading cause of rework.
- **Keep Informed roles lightweight**: Use async updates (status emails, board comments) rather than synchronous meetings for Informed roles.
