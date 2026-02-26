# OctoAcme — RACI Template

## Purpose
The RACI template clarifies who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed for key activities across the project lifecycle. A completed RACI reduces handoff confusion and ensures no activity is left without a clear owner.

## RACI Key
| Letter | Role | Meaning |
|--------|------|---------|
| **R** | Responsible | Does the work to complete the activity |
| **A** | Accountable | Ultimately answerable for the outcome; approves the deliverable; only one A per activity |
| **C** | Consulted | Provides input before or during the activity; two-way communication |
| **I** | Informed | Kept up to date on progress or outcomes; one-way communication |

## Roles Abbreviations
| Abbreviation | Role |
|---|---|
| Dev | Developer |
| PM-Prod | Product Manager |
| PM-Proj | Project Manager |
| UX | UX Designer |
| BA | Business Analyst |
| QA | QA Lead |
| DevOps | DevOps Engineer |

---

## RACI Matrix

| Activity | Dev | PM-Prod | PM-Proj | UX | BA | QA | DevOps |
|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | |
| Define problem statement & goals | C | A | C | C | R | I | I |
| Identify stakeholders & communication plan | I | C | A | I | C | I | I |
| Complete project one-pager | I | R | A | C | C | I | I |
| Go/no-go decision to enter planning | I | C | A | I | I | I | I |
| **Planning** | | | | | | | |
| Backlog creation & prioritization | C | A | C | C | R | C | I |
| Acceptance criteria authoring | C | C | A | C | R | C | I |
| Effort estimation | R | C | A | C | C | C | C |
| Define Definition of Done | C | C | A | I | C | R | C |
| Create RAID Log (initial entries) | C | C | A | I | C | C | R |
| Release plan & milestone map | C | C | A | I | I | C | C |
| **Execution** | | | | | | | |
| Feature development | R | I | I | C | C | C | C |
| UX design & handoff | C | C | I | R | C | I | I |
| Requirements clarification | C | C | I | C | R | C | I |
| Code review | R | I | I | I | I | C | C |
| CI/CD pipeline maintenance | I | I | I | I | I | C | R |
| RAID Log weekly review | C | C | A | I | C | C | C |
| Blocker escalation | R | C | A | I | I | C | C |
| **Quality & Testing** | | | | | | | |
| Test plan authoring | C | I | C | I | C | R | C |
| Unit & integration testing | R | I | I | I | I | C | I |
| QA / acceptance testing | C | C | C | C | C | R | C |
| Security scanning in CI | C | I | I | I | I | C | R |
| Quality gate sign-off before release | I | C | C | I | I | R | C |
| **Release & Deployment** | | | | | | | |
| Release notes authoring | R | C | A | I | C | C | I |
| Pre-release checklist sign-off | C | C | A | I | I | R | R |
| Deployment to staging | C | I | I | I | I | C | R |
| Deployment to production | C | I | A | I | I | C | R |
| Rollback decision & execution | C | I | A | I | I | C | R |
| Stakeholder release announcement | I | R | A | I | I | I | I |
| **Retrospective** | | | | | | | |
| Facilitate retrospective | C | C | R | C | C | C | C |
| Capture action items | R | R | A | R | R | R | R |
| Follow up on action items | C | C | A | C | C | C | C |

---

## How to Use This Template
1. Copy this table into your project's planning artifacts or project management tool.
2. Confirm role assignments with the full team at project kickoff.
3. Update the matrix when roles change or new activities are added.
4. Reference this matrix in sprint planning and handoff discussions to resolve ownership ambiguity.
5. Cross-reference with [Roles & Personas](./octoacme-roles-and-personas.md) for full role descriptions.

---

*Reviewed and agreed at project kickoff. Owner: Project Manager.*
