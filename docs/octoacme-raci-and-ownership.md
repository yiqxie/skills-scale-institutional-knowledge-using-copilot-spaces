# OctoAcme — RACI & Ownership Reference

## Purpose
A concise ownership and handoff checklist mapping each lifecycle stage to the accountable role, the required artifact, and the escalation contact.

See [OctoAcme Personas](octoacme-roles-and-personas.md) for full role definitions.

---

## Ownership by Lifecycle Stage

### Initiation

| Artifact | Accountable Role | Escalation Contact |
|---|---|---|
| Project One-pager | Product Manager | Executive Sponsor |
| Stakeholder list & communication plan | Project Manager | Executive Sponsor |
| Go/no-go decision | Executive Sponsor | — |
| Initial risk list | Project Manager | Product Manager |

**Handoff gate:** Executive Sponsor approves go/no-go before Planning begins.

---

### Planning

| Artifact | Accountable Role | Escalation Contact |
|---|---|---|
| Project plan & milestones | Project Manager | Product Manager |
| Technical design / architecture | Engineering Manager / Tech Lead | Executive Sponsor |
| Sprint backlog & acceptance criteria | Product Manager | Project Manager |
| UX research & design specs | UX / Design Researcher | Product Manager |
| Metric instrumentation plan | Data / Analytics Partner | Product Manager |
| Security requirements review | Security / Compliance Reviewer | Engineering Manager |

**Handoff gate:** Project Manager confirms plan is reviewed and baselined before Execution begins.

---

### Execution

| Artifact | Accountable Role | Escalation Contact |
|---|---|---|
| Feature implementation | Developer | Engineering Manager / Tech Lead |
| Test plans & QA sign-off | QA / Test Engineer | Project Manager |
| Risk register updates | Project Manager | Product Manager → Executive Sponsor |
| CI security scan results | Security / Compliance Reviewer | Engineering Manager |
| Dashboard & telemetry | Data / Analytics Partner | Product Manager |

**Escalation path:** Team → Project Manager → Product Lead → Executive Sponsor (Level 1 → 2 → 3)

---

### Release

| Artifact | Accountable Role | Escalation Contact |
|---|---|---|
| Pre-release checklist | Release Manager / Coordinator | Project Manager |
| Release notes | Release Manager / Coordinator | Product Manager |
| Security gate sign-off | Security / Compliance Reviewer | Engineering Manager |
| QA release readiness sign-off | QA / Test Engineer | Release Manager |
| Stakeholder & support announcements | Release Manager / Coordinator | Project Manager |
| Incident response & rollback | Support / On-call Engineer | Release Manager → Engineering Manager |

**Handoff gate:** Release Manager confirms all pre-release criteria are met before deploying to production.

---

### Retrospective

| Artifact | Accountable Role | Escalation Contact |
|---|---|---|
| Retrospective notes & action items | Project Manager | Product Manager |
| Post-release metric analysis | Data / Analytics Partner | Product Manager |
| Post-incident report (if applicable) | Support / On-call Engineer | Engineering Manager |

---

## Quick Escalation Reference

| Level | Trigger | Contact |
|---|---|---|
| Level 1 | Team-level blocker | Team triage in daily standup |
| Level 2 | Unresolved after 1 day; cross-team dependency | Project Manager → Product Manager / Product Lead |
| Level 3 | Business-impacting; funding or scope decision needed | Executive Sponsor |
| Security incident | Active security vulnerability or breach | Security / Compliance Reviewer → Security on-call |
