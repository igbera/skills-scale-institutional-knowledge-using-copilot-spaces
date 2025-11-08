# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min, facilitated by Scrum Master) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone (Scrum Master facilitates, QA Lead validates quality)

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval from Developer before merging (or team-defined policy)
  - For UI changes, request review from UX Designer
  - Tag QA Lead for items requiring manual QA validation

### Handoff: Development to QA
When a feature is ready for QA testing:
1. Developer moves item to "QA" column on project board
2. Developer ensures all acceptance criteria are documented
3. Developer notifies QA Lead with test instructions and edge cases to verify
4. QA Lead validates against acceptance criteria and Definition of Done
5. If issues found: QA Lead creates bugs linked to original issue, moves item back to "In Progress"
6. If passed: QA Lead approves and moves to "Done"

See [QA Handoff Checklist](./qa-handoff-checklist.md) for detailed process.

## Quality & Testing
- Unit tests for new logic (Developer responsibility)
- Integration tests where applicable (Developer with QA Lead guidance)
- End-to-end smoke tests for critical flows before release (QA Lead)
- Security scanning in CI (automated with Developer/QA review)
- Manual QA for feature acceptance when needed (QA Lead coordinates)
- UX validation for user-facing features (UX Designer)

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (Scrum Master facilitates)
- Level 2: Project Manager escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues
- Scrum Master tracks all blockers and ensures timely resolution

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled (Scrum Master owns calendar)
- [ ] Risk register updated weekly (Project Manager)
- [ ] QA handoff process established (QA Lead)
- [ ] Design review process in place (UX Designer)

_Updated to clarify role handoffs per [issue #4](https://github.com/igbera/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4)._
