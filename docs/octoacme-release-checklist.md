# OctoAcme — Release Checklist

## Purpose
Provide the Release Manager with a repeatable, step-by-step checklist to plan, coordinate, and complete a release with minimal risk. This checklist supplements the broader guidance in `docs/octoacme-release-and-deployment.md`.

## When to Use
Complete this checklist for every Patch, Minor, and Major release before deployment begins.

---

## Pre-Release (≥ 2 days before deployment)

- [ ] Release scope confirmed with Product Manager (features, fixes included)
- [ ] Release branch or tag created and named per convention (e.g. `release/v1.2.0`)
- [ ] Deployment window agreed with Project Manager and communicated to stakeholders
- [ ] QA Lead has provided written release-readiness sign-off
- [ ] All required PRs merged; CI pipeline passing on release branch
- [ ] Security scans completed with no critical open findings
- [ ] Release notes drafted and reviewed by Technical Writer
- [ ] Rollback plan documented and shared with the on-call team
- [ ] Customer Support Lead briefed on known issues and FAQs updated

## Deployment Day

- [ ] Pre-deployment backup or snapshot taken (if applicable)
- [ ] Staging deployment completed and smoke tests passed
- [ ] Go/No-Go decision confirmed by Release Manager, QA Lead, and Project Manager
- [ ] Production deployment initiated (automated pipeline preferred)
- [ ] Post-deployment smoke tests and monitoring checks completed
- [ ] Release notes and changelog published (internal and/or external)
- [ ] Stakeholders and Customer Support Lead notified of successful release

## Post-Release (within 48 hours)

- [ ] Post-release monitoring reviewed (errors, performance, support tickets)
- [ ] Any critical issues escalated immediately; rollback triggered if necessary
- [ ] Post-release retrospective scheduled and action items captured
- [ ] Release artifacts (notes, checklist, deployment log) archived in the project repo

---

## Rollback Trigger Criteria
Initiate rollback if any of the following are observed post-deployment:
- Error rate exceeds agreed threshold
- Core user workflows are non-functional
- Critical security vulnerability is discovered in the release
- Data integrity issues are detected

## Contacts
| Role | Responsibility |
|------|---------------|
| Release Manager | Owns checklist execution and go/no-go decision |
| QA Lead | Provides release-readiness sign-off |
| Project Manager | Coordinates timeline and stakeholder communication |
| Developer (on-call) | Executes deployment steps and rollback if required |
| Customer Support Lead | Prepares support team; monitors post-release tickets |
