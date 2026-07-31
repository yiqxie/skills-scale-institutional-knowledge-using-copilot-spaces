# OctoAcme Project Management Docs

This folder is the entry point for OctoAcme's project management process documentation. Use it to understand how projects move from idea to delivery, who owns which decisions, and which supporting artifacts keep work aligned.

## Overview

OctoAcme runs cross-functional projects through a lightweight lifecycle built around customer value, clear ownership, iterative delivery, and continuous learning. Work moves through five stages: **Initiation**, **Planning**, **Execution**, **Release**, and **Close & Retrospective**.

1. **Initiation** — validate the business need with a Project One-pager that captures the problem statement, SMART objective, success metrics, stakeholders, timeline, and initial risks before a go/no-go decision.
2. **Planning** — turn the approved initiative into a prioritized, estimated backlog with acceptance criteria, a documented Definition of Done, a release plan, and mapped dependencies.
3. **Execution** — deliver against the project board workflow (**Backlog → Ready → In Progress → In Review → QA → Done**) using small pull requests, linked issues, green CI, and required review approvals.
4. **Release** — clear pre-release gates, deploy through the agreed rollout process, verify production behavior, and communicate updates to stakeholders.
5. **Close & Retrospective** — capture learnings after each sprint, release, milestone, or incident and convert them into a small set of tracked follow-up actions.

## Roles and ownership

Every project has a named **Project Manager** and **Product Lead/Product Manager**. Product Managers define the problem, success metrics, priorities, and customer value outcomes. Project Managers own delivery plans, timelines, risk tracking, decision logs, and cross-team coordination. Developers implement against acceptance criteria, add tests and documentation, review code, and raise technical risks early. QA validates feature acceptance, while stakeholders and sponsors provide inputs, approvals, and escalation support.

## Communication cadence

OctoAcme uses a layered communication model: daily 15-minute standups for progress and blockers, weekly delivery syncs, weekly PM–PdM alignment, sprint or milestone demos, and monthly stakeholder updates. Teams maintain a single source of truth in the project README or release documentation, and use a standard weekly status update to share progress, next steps, risks or blockers, and decisions needed. Risks are tracked in a risk register and reviewed continuously through an identify → assess → mitigate → monitor cycle with tiered escalation when issues grow beyond team-level triage.

## Quality assurance and release discipline

Quality is built into delivery through unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for acceptance. Before release, teams confirm acceptance criteria are complete, pull requests are merged, CI and security scans pass, release notes are drafted, rollback plans are documented, and smoke tests are ready. If a release fails, the rollback and incident playbooks are used, followed by a blameless retrospective and tracked improvement actions.

## Documents in this folder

- [Project Management Overview](./octoacme-project-management-overview.md) — Introduces the shared principles, roles, artifacts, lifecycle, and baseline communication cadence.
- [Project Initiation Guide](./octoacme-project-initiation.md) — Defines the one-pager, minimum deliverables, initiation checklist, and approval gate for new work.
- [Project Planning](./octoacme-project-planning.md) — Covers kickoff activities, backlog structure, estimation, Definition of Done, and planning readiness checks.
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — Explains team rhythm, board workflow, pull request expectations, quality practices, and blocker escalation.
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — Describes the risk register, communication templates, update cadence, and escalation paths.
- [Release & Deployment Guide](./octoacme-release-and-deployment.md) — Documents release types, pre-release requirements, deployment steps, rollback guidance, and release notes.
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — Outlines retrospective timing, facilitation, action item tracking, and improvement culture.
- [Roles & Personas](./octoacme-roles-and-personas.md) — Defines the responsibilities, goals, and communication patterns for Developers, Product Managers, and Project Managers.

## How to use these docs

- Start with the [Project Management Overview](./octoacme-project-management-overview.md), then follow the lifecycle documents in order as a project matures.
- Keep the Project Charter or Project One-pager up to date in the project repository so status, scope, and success metrics stay current.
- Use these documents as context in Copilot Spaces when you want role-specific guidance, planning support, or process-aware outputs.
- Return to the release and retrospective guides at delivery milestones so lessons learned become tracked follow-up work.
