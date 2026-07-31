# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Role Summary Table

| Role | Primary Artifacts Owned | Escalation Level |
|---|---|---|
| Developer | Code, PRs, unit/integration tests, technical docs | Level 1 (team triage) |
| Product Manager | Product one-pager, roadmap, acceptance criteria | Level 2 (Product Lead) |
| Project Manager | Project plan, risk register, status reports | Level 2 (Product Lead) |
| QA / Test Engineer | Test plans, QA sign-off, defect reports | Level 2 (PM) |
| Release Manager / Release Coordinator | Release plan, deployment checklist, rollback plan, release notes | Level 2 (PM / Product Lead) |
| Engineering Manager / Tech Lead | Technical design docs, code review standards, capacity estimates | Level 2 (Product Lead) |
| Executive Sponsor | Go/no-go decisions, funding approval | Level 3 (Sponsor — final) |
| Stakeholder / Business Partner | Business requirements, approvals, stakeholder updates | Level 2 (PM) |
| Support / On-call Engineer | Incident response runbook, rollback logs | Level 2 (Release Manager / PM) |
| Security / Compliance Reviewer | Security scan results, compliance sign-off | Level 2 (PM / Engineering Manager) |
| UX / Design Researcher | Design specs, usability reports, research findings | Level 1–2 (PM) |
| Data / Analytics Partner | Dashboards, metric instrumentation, success measurement reports | Level 1–2 (PM) |

---

## RACI Table — Lifecycle Stages

**R** = Responsible, **A** = Accountable, **C** = Consulted, **I** = Informed

| Role | Initiation | Planning | Execution | Release | Retrospective |
|---|---|---|---|---|---|
| Developer | I | C | R | C | C |
| Product Manager | A | A | C | C | A |
| Project Manager | C | R | A | C | A |
| QA / Test Engineer | I | C | R | R | C |
| Release Manager / Coordinator | I | C | C | A | C |
| Engineering Manager / Tech Lead | C | R | C | C | C |
| Executive Sponsor | A | I | I | I | I |
| Stakeholder / Business Partner | C | I | I | I | I |
| Support / On-call Engineer | I | I | I | R | C |
| Security / Compliance Reviewer | C | C | C | R | I |
| UX / Design Researcher | C | R | C | I | C |
| Data / Analytics Partner | I | C | C | C | R |

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Interaction with Existing Roles
- Takes direction on scope and priorities from the **Product Manager**
- Reports progress and raises blockers to the **Project Manager**
- Collaborates with **QA / Test Engineers** on acceptance criteria and testability
- Receives technical guidance from the **Engineering Manager / Tech Lead**
- Partners with **UX / Design Researchers** to refine usability requirements

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Interaction with Existing Roles
- Collaborates with **Project Managers** on scheduling and dependency management
- Provides requirements and priorities to **Developers**
- Partners with **UX / Design Researchers** for problem validation and usability studies
- Aligns roadmap and go/no-go decisions with the **Executive Sponsor**
- Keeps **Stakeholders / Business Partners** informed via roadmap updates and briefings
- Works with **Data / Analytics Partners** to define and monitor success metrics

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Interaction with Existing Roles
- Works daily with **Developers** to unblock issues and track delivery
- Aligns scope and priorities with the **Product Manager**
- Escalates to the **Executive Sponsor** for Level 3 business-impacting issues
- Coordinates release logistics with the **Release Manager / Release Coordinator**
- Routes security concerns to the **Security / Compliance Reviewer**
- Keeps **Stakeholders / Business Partners** informed through status reports

---

## QA / Test Engineer

### Role Summary
Validates that delivered increments meet acceptance criteria and quality standards before release.

### Responsibilities
- Define and maintain test plans and the QA approach for each milestone
- Execute manual feature acceptance and end-to-end smoke tests
- Verify Definition of Done is met prior to release sign-off
- Report defects with clear reproduction steps and severity
- Maintain a regression suite and flag coverage gaps

### Goals
- Prevent regressions from reaching production
- Shorten feedback loops between development and validation

### Typical Communication
- Daily standups, test status in weekly delivery sync, release readiness sign-off

### Interaction with Existing Roles
- Works with **Developers** on testability and acceptance criteria
- Confirms scope coverage with the **Product Manager**
- Reports release readiness and blockers to the **Project Manager**
- Coordinates final release sign-off with the **Release Manager / Release Coordinator**

---

## Release Manager / Release Coordinator

### Role Summary
Owns the release process end-to-end — from scheduling deployment windows to coordinating rollback procedures and communicating release outcomes.

### Responsibilities
- Define and maintain the release calendar and deployment windows
- Own the pre-release checklist and coordinate readiness across teams
- Draft and publish release notes for each release
- Maintain and execute the rollback plan when a deployment fails
- Announce releases to stakeholders and the support team

### Goals
- Ensure predictable, low-risk deployments to production
- Keep stakeholders and support informed of release status
- Minimize mean-time-to-recovery when incidents occur

### Typical Communication
- Release readiness meetings, Slack announcements, release notes distribution

### Interaction with Existing Roles
- Partners with **Developers** and **QA / Test Engineers** to confirm pre-release readiness
- Coordinates scheduling and scope with the **Project Manager** and **Product Manager**
- Notifies **Support / On-call Engineers** before each deployment and during incidents
- Engages the **Security / Compliance Reviewer** to confirm security scan gates are passed

---

## Engineering Manager / Tech Lead

### Role Summary
Provides technical direction and oversight, ensuring code quality, sound architecture, and realistic capacity estimates for the delivery team.

### Responsibilities
- Set and maintain code review standards and engineering best practices
- Drive technical design decisions and architecture reviews
- Provide capacity estimates and help with sprint planning
- Identify and mitigate technical debt and architectural risks
- Support developer growth through mentoring and feedback

### Goals
- Keep the codebase maintainable, scalable, and secure
- Align technical decisions with product and business goals

### Typical Communication
- Architecture review meetings, PR review threads, planning sessions

### Interaction with Existing Roles
- Guides **Developers** on technical direction and code quality
- Consults with the **Product Manager** to evaluate technical feasibility and trade-offs
- Provides capacity and estimate input to the **Project Manager**
- Collaborates with the **Security / Compliance Reviewer** on architectural security decisions
- Works with **QA / Test Engineers** to establish quality gates and testing standards

---

## Executive Sponsor

### Role Summary
Provides executive-level authority, funding, and final approval at key decision gates. Acts as the Level 3 escalation contact for business-impacting issues.

### Responsibilities
- Approve the go/no-go decision at project initiation
- Secure funding and resources for the project
- Resolve escalations that cannot be addressed at the PM or Product Lead level
- Align project goals with broader organizational strategy
- Champion the project within executive leadership

### Goals
- Ensure the project delivers measurable business value
- Unblock critical decisions quickly to keep delivery on track

### Typical Communication
- Milestone briefings, executive dashboards, Level 3 escalation notifications

### Interaction with Existing Roles
- Receives go/no-go recommendations from the **Product Manager** and **Project Manager**
- Acts as final escalation contact when the **Project Manager** and **Product Manager** cannot resolve a blocker
- Kept informed by the **Project Manager** through milestone reports
- Authorizes resource or scope changes requested by the **Product Manager**

---

## Stakeholder / Business Partner

### Role Summary
Represents business functions (sales, support, marketing, legal, finance) that provide inputs, approvals, and consume status updates throughout the project lifecycle.

### Responsibilities
- Provide business requirements and constraints to the product and delivery team
- Review and approve key milestones and release readiness from a business perspective
- Surface market or customer signals relevant to scope and priority
- Consume and share project status updates within their business unit

### Goals
- Ensure the project meets business needs and readiness criteria
- Enable their teams to prepare for the release (training, communications, support)

### Typical Communication
- Monthly stakeholder updates, milestone-based reviews, release announcements

### Interaction with Existing Roles
- Provides inputs and approvals to the **Product Manager**
- Receives status updates from the **Project Manager**
- Coordinates support readiness and announcements with the **Release Manager / Release Coordinator**

---

## Support / On-call Engineer

### Role Summary
First responder during incidents and deployment rollbacks. Monitors production health and executes the incident response runbook when issues arise.

### Responsibilities
- Monitor alerts and respond to production incidents
- Execute rollback steps when a deployment causes critical issues
- Triage and communicate incident status to stakeholders
- Capture action items and contribute to post-incident retrospectives
- Maintain and improve the on-call runbook

### Goals
- Minimize customer impact during incidents
- Restore production to a known-good state as quickly as possible

### Typical Communication
- Incident channels, on-call handoff notes, post-incident reports

### Interaction with Existing Roles
- Works directly with the **Release Manager / Release Coordinator** during deployments and incidents
- Escalates unresolved incidents to the **Engineering Manager / Tech Lead** and **Project Manager**
- Provides post-incident findings to **Developers** for root-cause fixes
- Keeps **Stakeholders / Business Partners** informed during extended incidents

---

## Security / Compliance Reviewer

### Role Summary
Ensures the project meets security and regulatory requirements. Reviews code, architecture, and processes for vulnerabilities and compliance gaps.

### Responsibilities
- Review security scanning results in CI and flag issues before release
- Conduct architecture and code reviews for security risks
- Define and maintain the security incident runbook
- Ensure compliance requirements are met at each lifecycle gate
- Act as Security on-call contact for active security incidents

### Goals
- Prevent security vulnerabilities from reaching production
- Ensure continuous compliance with applicable regulations and standards

### Typical Communication
- Security review meetings, scan reports, incident notifications

### Interaction with Existing Roles
- Partners with **Developers** and the **Engineering Manager / Tech Lead** on secure coding practices
- Provides security gate sign-off to the **Release Manager / Release Coordinator** before each release
- Advises the **Project Manager** on security-related risks and timeline impacts
- Reports active security incidents to the **Executive Sponsor** when warranted

---

## UX / Design Researcher

### Role Summary
Validates that the product solves real user problems and meets usability standards. Translates user research into actionable design requirements and success criteria.

### Responsibilities
- Conduct user research and usability studies to validate problem statements
- Define usability success criteria and design acceptance criteria
- Create wireframes, prototypes, and design specifications
- Partner with Product to prioritize research findings in the backlog
- Evaluate delivered features against usability benchmarks

### Goals
- Ensure delivered features are usable and meet user needs
- Provide evidence-based inputs to product and engineering decisions

### Typical Communication
- Research readout meetings, design reviews, usability test reports

### Interaction with Existing Roles
- Collaborates with the **Product Manager** on problem validation and acceptance criteria
- Works with **Developers** to ensure designs are implemented accurately
- Shares usability findings with **Stakeholders / Business Partners** to inform go-to-market plans
- Coordinates with **QA / Test Engineers** to incorporate usability checks in acceptance testing

---

## Data / Analytics Partner

### Role Summary
Instruments and monitors success metrics, maintains dashboards, and provides data insights that drive product and project decisions.

### Responsibilities
- Define and implement metric instrumentation for new features
- Build and maintain dashboards tracking key project success metrics
- Analyze data to validate outcomes and identify improvement opportunities
- Partner with Product to define measurable success criteria
- Support post-release analysis and retrospective data reviews

### Goals
- Ensure every major release has measurable success criteria tracked in a dashboard
- Enable data-driven decisions across the product lifecycle

### Typical Communication
- Data reviews in weekly delivery syncs, retrospective metric summaries, dashboard links in status reports

### Interaction with Existing Roles
- Collaborates with the **Product Manager** to define and monitor success metrics
- Provides instrumentation guidance to **Developers** for telemetry implementation
- Shares post-release metric analysis with the **Project Manager** for retrospectives
- Supports **Executive Sponsor** reporting with high-level dashboard summaries

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

