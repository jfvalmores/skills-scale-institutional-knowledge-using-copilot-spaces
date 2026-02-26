# OctoAcme — RAID Log Template

## Purpose
The RAID Log tracks four categories of project management concerns: **R**isks, **A**ssumptions, **I**ssues, and **D**ependencies. Maintaining a single, up-to-date RAID Log provides a shared source of truth for the delivery team and stakeholders, and reduces the likelihood of surprises derailing the project.

## Ownership
- **Project Manager** owns the RAID Log and ensures it is reviewed at least weekly during the delivery sync.
- **All team members** are responsible for raising new entries as they are discovered.
- Individual entries are assigned an **Owner** who is accountable for monitoring and actioning the item.

## Review Cadence
| Cadence | Activity |
|---------|----------|
| Daily standup | Flag any new high-severity risks or blocking issues |
| Weekly delivery sync | Full RAID review — update statuses, confirm ownership, close resolved items |
| Sprint / milestone end | Archive closed items; carry forward open items with refreshed priorities |
| Release gate | Confirm no open blocking Issues or high-probability Risks before deployment |

---

## Risks

Risks are uncertain events or conditions that, if they occur, could negatively affect project objectives.

| ID | Description | Impact (H/M/L) | Probability (H/M/L) | Owner | Mitigation Plan | Status | Date Raised | Date Updated |
|----|-------------|---------------|---------------------|-------|-----------------|--------|-------------|--------------|
| R-001 | _Example: Key developer unavailable during critical sprint_ | H | M | Project Manager | Cross-train a second developer; adjust sprint scope | Open | YYYY-MM-DD | YYYY-MM-DD |

**Status values**: Open · Mitigated · Accepted · Closed

---

## Assumptions

Assumptions are conditions believed to be true for planning purposes but not yet confirmed. If an assumption proves false, it may become a risk or issue.

| ID | Description | Owner | Validation Approach | Validation Due | Status | Date Raised | Date Updated |
|----|-------------|-------|---------------------|---------------|--------|-------------|--------------|
| A-001 | _Example: Third-party API will maintain backward compatibility through Q3_ | Business Analyst | Review API changelog and contact vendor | YYYY-MM-DD | Open | YYYY-MM-DD | YYYY-MM-DD |

**Status values**: Open · Validated · Invalidated (escalate to Risk/Issue) · Closed

---

## Issues

Issues are problems that have already occurred and require active resolution. Unlike risks, they are current and impacting the project now.

| ID | Description | Impact (H/M/L) | Owner | Resolution Plan | Target Resolution Date | Status | Date Raised | Date Updated |
|----|-------------|---------------|-------|-----------------|----------------------|--------|-------------|--------------|
| I-001 | _Example: Staging environment unavailable — blocking QA testing_ | H | DevOps Engineer | Rebuild staging environment from IaC scripts | YYYY-MM-DD | In Progress | YYYY-MM-DD | YYYY-MM-DD |

**Status values**: Open · In Progress · Resolved · Escalated · Closed

**Escalation path**: Team-level → Project Manager → Product Lead → Sponsor (see [Execution & Tracking](./octoacme-execution-and-tracking.md) for full escalation levels)

---

## Dependencies

Dependencies are conditions, deliverables, or decisions that the project relies on — either from within the team or from external parties.

| ID | Description | Type (Internal/External) | Depends On (Team/System/Party) | Owner | Due Date | Status | Date Raised | Date Updated |
|----|-------------|--------------------------|-------------------------------|-------|----------|--------|-------------|--------------|
| D-001 | _Example: Design handoff from UX Designer required before front-end development can begin_ | Internal | UX Designer | Project Manager | YYYY-MM-DD | Pending | YYYY-MM-DD | YYYY-MM-DD |

**Status values**: Pending · In Progress · Resolved · At Risk · Closed

---

## Archiving Closed Items
- Move resolved/closed entries to an **Archive** section (or a separate archived sheet) at each milestone end.
- Retain for reference during retrospectives and post-project reviews.

---

*Maintain this log in the project repository or project management tool. Reference it in [Project Planning](./octoacme-project-planning.md) and [Execution & Tracking](./octoacme-execution-and-tracking.md).*
