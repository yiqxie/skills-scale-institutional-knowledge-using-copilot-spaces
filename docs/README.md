# OctoAcme Project Management Docs

## Overview
OctoAcme uses a five-stage lifecycle for delivery: **Initiation, Planning, Execution, Release, and Close/Retrospective**. Initiation validates business need through a Project One-pager that captures the problem statement, SMART objective, success metrics, stakeholders, timeline, and initial risks, then applies a go/no-go decision gate. Planning turns approved work into a prioritized, estimated backlog with acceptance criteria, a documented Definition of Done, a release plan and milestone map, plus tracked dependencies.

Execution is managed through a project board flow (**Backlog → Ready → In Progress → In Review → QA → Done**) and a disciplined PR workflow: keep PRs small (≤400 lines when possible), include issue links and acceptance criteria in descriptions, run CI tests/lint before review, and require at least one approval before merge. Releases are categorized as patch, minor, or major and follow a checklist that includes staging smoke tests, automated production deployment, post-deploy verification, stakeholder communication, and a documented rollback plan.

Ownership is explicit across personas: **Project Manager, Product Manager, Developers, QA/Testing, and Stakeholders**. The operating principles are customer-first prioritization, iterative delivery, clear ownership, data-informed decisions, and psychological safety. These persona definitions are reusable in Copilot Spaces as role-specific prompts for planning, execution, and communication support.

Communication and risk management follow a standard cadence: daily 15-minute standups, weekly delivery sync, weekly PM + PdM alignment, sprint-end demos, and monthly stakeholder updates. Teams use a Weekly Status template (progress, next steps, risks & blockers, asks/decisions) and maintain a Risk Register (ID, description, impact, likelihood, owner, mitigation, status) through identify → assess → mitigate → monitor. Quality and improvement are continuous through unit/integration/E2E smoke tests, CI security scanning, manual QA for acceptance, and retrospective timeboxes (45–75 minutes) that produce 2–3 tracked action items with owners and due dates, reviewed in weekly PM syncs.

## Documents
- [Project Management Overview](./octoacme-project-management-overview.md) — principles, core roles, key artifacts, lifecycle, and communication cadence.
- [Project Initiation](./octoacme-project-initiation.md) — one-pager template, minimum deliverables, initiation checklist, and decision gate.
- [Project Planning](./octoacme-project-planning.md) — kickoff, backlog item template, estimation, DoD, and planning checklist.
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — team rhythm, PR workflow, quality & testing, metrics, and blocker escalation.
- [Risks & Communication](./octoacme-risks-and-communication.md) — risk register, risk lifecycle, status/incident templates, and escalation paths.
- [Release & Deployment](./octoacme-release-and-deployment.md) — release types, pre-release requirements, deployment checklist, rollback playbook, and release notes template.
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — retro structure, facilitation tips, and action item tracking.
- [Roles & Personas](./octoacme-roles-and-personas.md) — Developers, Product Managers, and Project Managers: responsibilities, goals, and communication.

## How to use these docs
1. Start with the [Project Management Overview](./octoacme-project-management-overview.md), then follow the lifecycle documents in order: Initiation → Planning → Execution & Tracking → Release & Deployment → Retrospective & Continuous Improvement.
2. Keep the Project Charter / One-pager updated in your project repository so status, scope, and success metrics stay current.
3. Add these docs to Copilot Spaces context and use the role/persona docs for role-specific guidance during planning, execution, risk handling, release, and retrospectives.
