# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- QA signoff obtained (all test cases passed, critical bugs resolved)
- UX Designer approval for user-facing changes
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared by QA Lead

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) - Project Manager
- [ ] Backup or snapshot (if applicable) - Developer/DevOps
- [ ] Deploy to staging and run smoke tests - QA Lead validates
- [ ] Deploy to production (automated pipeline preferred) - Developer/DevOps
- [ ] Run post-deploy verifications - QA Lead confirms
- [ ] Announce release to stakeholders and support - Project Manager
- [ ] Update documentation if needed - Technical Writer/Developer

### QA Signoff for Release
Before a release can be deployed to production, the QA Lead must verify:
- [ ] All planned features tested and approved
- [ ] Critical and high-priority bugs resolved
- [ ] Regression testing completed for affected areas
- [ ] Performance and security scans reviewed
- [ ] UAT completed (if applicable) with Product Manager/stakeholders
- [ ] Smoke test results documented
- [ ] Known issues documented in release notes

QA Lead provides formal signoff via release tracking issue or project board comment.

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (Project Manager coordinates)
  - Rollback to last known-good release if necessary (Developer/DevOps executes)
  - Triage root cause and capture action items (QA Lead participates in analysis)
  - Schedule incident retrospective (Scrum Master facilitates)

_Updated to include QA signoff requirements per [issue #4](https://github.com/igbera/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4)._

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
