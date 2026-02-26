# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

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

---

## UX Designer

### Role Summary
UX Designers translate user needs and business goals into intuitive, accessible product experiences. They bridge the gap between product vision and engineering implementation through research, prototyping, and design specifications.

### Responsibilities
- Conduct user research and synthesize findings into actionable insights
- Create wireframes, prototypes, and high-fidelity design specifications
- Collaborate with Product Managers on feature scoping and acceptance criteria
- Define and maintain design standards and component libraries
- Review implemented features for design fidelity and usability
- Advocate for accessibility (WCAG compliance) and inclusive design

### Goals
- Deliver clear, user-validated designs that reduce rework
- Minimize ambiguity between design intent and implementation
- Ensure consistent, accessible user experiences across the product

### Typical Communication
- Design reviews and handoff sessions with Developers
- Regular syncs with Product Managers on scope and priorities
- Usability test readouts to stakeholders
- Annotations and notes within design files (e.g., Figma)

### Interactions with Existing Roles
- **Developers**: Hands off design specs and assets; reviews PRs for visual and interaction accuracy; clarifies design intent during implementation.
- **Product Managers**: Collaborates on problem framing, user stories, and acceptance criteria; validates designs against product goals.
- **Project Managers**: Flags design dependencies and capacity needs during planning; participates in sprint planning and demos.

---

## Business Analyst

### Role Summary
Business Analysts bridge business needs and technical solutions. They elicit, document, and validate requirements, ensuring that what is built aligns with stakeholder expectations and delivers measurable value.

### Responsibilities
- Elicit and document functional and non-functional requirements
- Produce process flows, use cases, and data dictionaries as needed
- Validate acceptance criteria with stakeholders and the delivery team
- Support UAT (User Acceptance Testing) planning and execution
- Identify gaps or conflicts in requirements and escalate early
- Maintain requirements traceability across the project lifecycle

### Goals
- Ensure requirements are unambiguous, complete, and testable
- Reduce downstream rework caused by unclear or missing requirements
- Bridge communication gaps between business stakeholders and engineering

### Typical Communication
- Requirements workshops and stakeholder interviews
- Written requirements artifacts (user stories, BRDs, process maps)
- Review sessions with Developers and QA Lead to validate test coverage
- Status updates to Project Managers on requirements completeness

### Interactions with Existing Roles
- **Developers**: Clarifies requirements during implementation; reviews acceptance criteria for technical feasibility.
- **Product Managers**: Supports backlog refinement and acceptance criteria authoring; aligns on priorities and scope boundaries.
- **Project Managers**: Reports requirements progress and flags open decisions or scope changes that affect timeline.

---

## QA Lead

### Role Summary
The QA Lead owns the quality strategy and testing practice for a project. They establish testing standards, coordinate quality gates, and ensure defects are caught before they reach production. This role complements the quality and testing guidance in [Execution & Tracking](./octoacme-execution-and-tracking.md) and [Release & Deployment](./octoacme-release-and-deployment.md).

### Responsibilities
- Define and maintain the test plan, including unit, integration, end-to-end, and regression strategies
- Own and maintain the Definition of Done (DoD) quality criteria — see [DoD template](./octoacme-definition-of-done.md)
- Coordinate manual and automated testing activities across sprints
- Triage and prioritize defects; escalate release-blocking issues
- Gate releases at quality checkpoints in collaboration with DevOps Engineer and Project Manager
- Track and report on test coverage, defect rates, and quality metrics

### Goals
- Prevent regressions and release-blocking defects
- Increase automated test coverage incrementally each sprint
- Maintain a clear, shared understanding of quality standards across the team

### Typical Communication
- Test plan review with Developers and Business Analyst at sprint start
- Defect triage and status updates in daily standup and weekly sync
- Quality gate sign-off before each release
- Test result reports for stakeholders and Project Managers

### Interactions with Existing Roles
- **Developers**: Collaborates on test strategy; reviews PR acceptance criteria for testability; escalates defects for immediate fix.
- **Product Managers**: Aligns on UAT requirements and acceptable defect thresholds for release.
- **Project Managers**: Reports quality status and flags go/no-go concerns; contributes to RAID log for quality risks — see [RAID Log template](./octoacme-raid-log-template.md).

---

## DevOps Engineer

### Role Summary
DevOps Engineers design and maintain the delivery pipeline, infrastructure, and operational tooling that enable the team to ship software reliably and repeatedly. They reduce the friction between development and operations.

### Responsibilities
- Build and maintain CI/CD pipelines (builds, tests, deployments)
- Manage cloud infrastructure, environments (dev, staging, production), and access controls
- Own incident response tooling, monitoring, alerting, and on-call runbooks
- Automate security scanning, dependency checks, and compliance gates in the pipeline
- Support the release process, including rollback procedures and deployment windows
- Collaborate on capacity planning and environment readiness

### Goals
- Maximize deployment frequency while minimizing failure rate and recovery time
- Reduce manual steps in the delivery process through automation
- Ensure observability and reliability of production systems

### Typical Communication
- Pipeline and environment status updates in weekly delivery sync
- Runbooks and infrastructure-as-code documentation in the repo
- Incident notifications and post-incident reviews with the broader team
- Deployment readiness sign-off with QA Lead and Project Manager

### Interactions with Existing Roles
- **Developers**: Supports local environment setup and CI troubleshooting; reviews infrastructure changes in PRs; guides best practices for containerization and secrets management.
- **Product Managers**: Communicates deployment constraints (e.g., maintenance windows, staged rollouts) that affect feature availability timelines.
- **Project Managers**: Flags infrastructure risks and dependencies in the RAID log — see [RAID Log template](./octoacme-raid-log-template.md); participates in release go/no-go decisions.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See the [RACI template](./octoacme-raci-template.md) for a view of role accountability across project phases.

