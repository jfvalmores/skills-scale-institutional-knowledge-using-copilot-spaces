# OctoAcme — Definition of Done (DoD)

## Purpose
The Definition of Done (DoD) establishes a shared, agreed-upon set of criteria that every work item (story, task, bug fix) must satisfy before it is considered complete. A consistent DoD reduces ambiguity, prevents rework, and maintains quality standards across sprints and releases.

## Ownership
- **QA Lead** owns and maintains this document.
- **Project Manager** ensures the DoD is agreed upon at the start of each project or major phase (see [Project Planning](./octoacme-project-planning.md)).
- **All team members** are responsible for applying the DoD before marking work as Done.

---

## DoD Checklist — Story / Task Level

### Code Quality
- [ ] Code written and peer-reviewed (at least one approval on the PR)
- [ ] PR is linked to the relevant issue and acceptance criteria are met
- [ ] No new linting errors or warnings introduced
- [ ] Code follows agreed conventions (naming, structure, formatting)

### Testing
- [ ] Unit tests written for new logic; all existing tests pass
- [ ] Integration tests updated or added where applicable
- [ ] No known regression introduced (confirmed via CI)
- [ ] Manual testing completed for UI changes or complex flows

### Security & Compliance
- [ ] Security scanning (SAST/dependency scan) passed in CI
- [ ] No new high/critical vulnerabilities introduced
- [ ] Sensitive data (secrets, PII) is not logged or exposed

### Documentation
- [ ] Inline code comments added where logic is non-obvious
- [ ] README or relevant doc updated if behavior or setup has changed
- [ ] API contract or schema changes documented (if applicable)

### Deployment Readiness
- [ ] Feature flag configured (if applicable)
- [ ] Migration scripts tested in a non-production environment (if applicable)
- [ ] CI pipeline passes (build, test, lint, scan)

---

## DoD Checklist — Sprint / Milestone Level

- [ ] All stories meeting story-level DoD are in the **Done** column on the project board
- [ ] Velocity and burndown reviewed; deviations noted
- [ ] Risks and action items from the sprint added or updated in the [RAID Log](./octoacme-raid-log-template.md)
- [ ] Demo delivered to stakeholders (or recording shared)
- [ ] Sprint retrospective completed and action items captured

---

## DoD Checklist — Release Level

- [ ] All stories in scope meet story-level DoD
- [ ] End-to-end / smoke tests passed on staging environment
- [ ] Release notes drafted and reviewed — see [Release & Deployment](./octoacme-release-and-deployment.md)
- [ ] Rollback plan documented and validated
- [ ] QA Lead sign-off obtained
- [ ] DevOps Engineer deployment readiness confirmed
- [ ] Stakeholder communication prepared

---

## Updating the DoD
- Review and update this checklist during retrospectives when recurring quality issues are identified.
- Changes require agreement from the QA Lead, Project Manager, and team.
- Version and date any significant changes at the bottom of this document.

---

*Last reviewed: see git history*
