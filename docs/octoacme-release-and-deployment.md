# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- All items in scope meet the [Definition of Done](./octoacme-definition-of-done.md)
- Passing CI and security scans
- Release notes drafted (owner: **Developer** drafts; **Project Manager** approves)
- Rollback / mitigation plan documented (owner: **DevOps Engineer**)
- Smoke tests prepared and signed off by **QA Lead**
- No open blocking Issues in the [RAID Log](./octoacme-raid-log-template.md)
- Deployment readiness confirmed by **DevOps Engineer** and **QA Lead**

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **DevOps Engineer** triggers incident response and notifies on-call
  - **Project Manager** coordinates stakeholder communication
  - **DevOps Engineer** executes rollback to last known-good release if necessary
  - **Developer** and **QA Lead** triage root cause and capture action items
  - Record the incident as an Issue in the [RAID Log](./octoacme-raid-log-template.md)

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
