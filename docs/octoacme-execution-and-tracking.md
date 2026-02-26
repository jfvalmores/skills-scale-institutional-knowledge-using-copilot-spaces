# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- All work must satisfy the [Definition of Done](./octoacme-definition-of-done.md) before being marked complete
- **QA Lead** owns quality gates; Developers are responsible for meeting DoD criteria before requesting review

## RAID Review Cadence
- **Daily standup**: flag any new high-severity risks or blocking issues immediately
- **Weekly delivery sync**: full RAID Log review — update statuses, confirm ownership, close resolved items
- **Sprint/milestone end**: archive closed items; carry forward open items with refreshed priorities
- Maintain the [RAID Log](./octoacme-raid-log-template.md) as the single source of truth for risks, assumptions, issues, and dependencies

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- **Level 1**: Developer or team member raises in daily standup; team resolves within the sprint
- **Level 2**: **Project Manager** escalates to Product Lead and dependent teams if unresolved within one working day
- **Level 3**: **Project Manager** triggers sponsor-level escalation for business-impacting issues; record escalation in the [RAID Log](./octoacme-raid-log-template.md)
- For security incidents, follow the security incident runbook and notify Security on-call immediately

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] RAID Log reviewed and updated weekly — see [RAID Log template](./octoacme-raid-log-template.md)
- [ ] Definition of Done applied to all completed items — see [DoD template](./octoacme-definition-of-done.md)
