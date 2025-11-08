# OctoAcme Project Management

Welcome to OctoAcme's project management documentation. This guide provides an overview of our project lifecycle, key workflows, roles, and communication practices—everything you need to successfully deliver projects at OctoAcme.

## Overview

OctoAcme follows a structured yet iterative project management approach built on customer-first principles and data-informed decision-making. Our lifecycle spans five key phases: **Initiation**, **Planning**, **Execution**, **Release**, and **Retrospective**. During Initiation, we validate business need and define success metrics through a lightweight Project One-pager. Planning transforms approved initiatives into actionable backlogs with clear acceptance criteria, estimates, and release milestones. Execution focuses on incremental delivery using project board workflows (Backlog → Ready → In Progress → In Review → QA → Done), daily standups, and weekly delivery syncs to track progress and escalate blockers. Release activities ensure safe, observable deployments through pre-release checklists, smoke tests, and rollback playbooks. Finally, we close with Retrospectives to capture learnings and convert them into continuous improvement action items.

Our workflows emphasize small, testable increments with clear pull request guidelines: PRs should be ≤400 lines when possible, include issue links and acceptance criteria, and pass automated tests and security scans before review. The project board tracks work through standardized columns, and at least one approval is required before merging. CI gates enforce unit tests, integration tests, and security scanning, while end-to-end smoke tests validate critical flows before release. When deployments encounter issues, our rollback playbook provides clear incident response steps and post-incident retrospectives.

Teams operate with well-defined personas and responsibilities. The **Project Manager (PM)** coordinates delivery, schedules, risk management, and communications. The **Product Manager (PdM)** defines outcomes, prioritizes the backlog, and measures success. **Developers** implement features with high test coverage and observability. **QA/Testing** validates quality against acceptance criteria. **Stakeholders** provide inputs, approvals, and business context. Communication follows a regular cadence: PM and PdM align weekly, the delivery team holds twice-weekly standups (or as agreed), stakeholders receive monthly updates, and ad-hoc escalations occur as needed. Risk management uses a simple register to track ID, description, impact, likelihood, owner, mitigation, and status, reviewed during weekly syncs.

Quality assurance is embedded throughout the lifecycle. Unit tests validate new logic, integration tests cover component interactions, and end-to-end smoke tests protect critical user flows before each release. Security scanning runs automatically in CI pipelines. Our release checklist ensures all acceptance criteria are met, CI and security scans pass, release notes are drafted, and rollback plans are documented. Post-deploy verification and stakeholder announcements complete the release process. If issues arise, our incident playbook guides rollback to the last known-good release, root cause triage, and action item capture to prevent recurrence.

## Process Documentation Index

Detailed guidance for each phase and topic:

- [OctoAcme Project Management Overview](octoacme-project-management-overview.md) — Principles, roles, artifacts, and high-level lifecycle
- [OctoAcme Project Initiation](octoacme-project-initiation.md) — Validate ideas, align stakeholders, create Project One-pagers
- [OctoAcme Project Planning](octoacme-project-planning.md) — Build actionable backlogs, estimate scope, define release plans
- [OctoAcme Execution & Tracking](octoacme-execution-and-tracking.md) — Daily standups, project board workflows, PR guidelines, CI practices
- [OctoAcme Risk Management & Communication](octoacme-risks-and-communication.md) — Risk registers, stakeholder updates, escalation paths
- [OctoAcme Release & Deployment](octoacme-release-and-deployment.md) — Pre-release checklists, deployment steps, rollback playbooks
- [OctoAcme Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) — Capture learnings, track action items
- [OctoAcme Roles & Personas](octoacme-roles-and-personas.md) — Detailed responsibilities for PM, PdM, Developers, QA, Stakeholders

## Acceptance Criteria

- [ ] Content aligns with existing process docs
- [ ] Update improves clarity or closes a documented gap
- [ ] Proposed content has been reviewed with stakeholders (if needed)
