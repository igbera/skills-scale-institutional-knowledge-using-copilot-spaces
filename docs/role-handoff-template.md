# Role Handoff Template

## Purpose
This template standardizes handoffs between roles to ensure clarity, accountability, and completeness. Use it whenever work transitions between roles to minimize confusion and rework.

---

## General Handoff Template

### From: [Role Name]
### To: [Role Name]
### Item: [Feature/Task/Deliverable Name]
### Date: [Handoff Date]

---

## Handoff Details

### What is being handed off
- **Summary**: [Brief description of the work item]
- **Status**: [Current state - e.g., complete, needs review, partially done]
- **Artifacts**: [Links to relevant documents, PRs, designs, etc.]

### What has been completed
- [ ] [Deliverable 1]
- [ ] [Deliverable 2]
- [ ] [Deliverable 3]

### What is expected next
- **Next steps**: [Clear description of what the receiving role should do]
- **Acceptance criteria**: [How the receiving role knows the work meets expectations]
- **Priority**: [High/Medium/Low]
- **Deadline**: [Target completion date, if applicable]

### Context and notes
- **Background**: [Relevant context, decisions made, constraints]
- **Risks/Concerns**: [Potential issues or areas needing attention]
- **Dependencies**: [Any blockers or items needed before proceeding]
- **Questions/Clarifications**: [Open items or areas needing input]

### Contacts
- **For questions contact**: [Name/Role]
- **Stakeholders to notify**: [List of people to keep informed]

---

## Common Handoff Scenarios

### Product Manager → Business Analyst
**What**: Initial feature concept for requirements analysis

**Handoff includes**:
- Product vision and business case
- Target users and use cases
- Success metrics
- Constraints and assumptions

**Business Analyst will**:
- Document detailed requirements
- Validate business value mapping
- Create functional specifications

---

### Business Analyst → UX Designer
**What**: Functional requirements for design

**Handoff includes**:
- User flows and scenarios
- Functional requirements document
- Business rules and validation logic
- Success metrics

**UX Designer will**:
- Create wireframes and prototypes
- Conduct user research
- Define UI specifications

---

### UX Designer → Developer
**What**: Design specifications for implementation

**Handoff includes**:
- Mockups and interactive prototypes
- Design system references
- Accessibility requirements
- Responsive behavior specifications

**Developer will**:
- Implement UI according to specs
- Request clarifications if needed
- Flag technical constraints

---

### Developer → QA Lead
**What**: Completed feature for testing

**Handoff includes**:
- Completed code merged to target branch
- Test instructions and edge cases
- Environment setup notes
- Acceptance criteria confirmation

**QA Lead will**:
- Execute test plan
- Validate acceptance criteria
- Report defects or approve for release

See also: [QA Handoff Checklist](./qa-handoff-checklist.md)

---

### QA Lead → Product Manager/Stakeholders
**What**: QA-approved feature for UAT or final approval

**Handoff includes**:
- QA test results and signoff
- Known issues or limitations
- User instructions or demo
- Deployment readiness confirmation

**Product Manager will**:
- Conduct UAT with stakeholders
- Validate business value delivered
- Approve for production release

---

### Project Manager → Scrum Master
**What**: Sprint-level planning details for execution

**Handoff includes**:
- Sprint goals and priorities
- Resource allocation
- Dependencies and risks
- Success criteria for the sprint

**Scrum Master will**:
- Facilitate sprint ceremonies
- Track progress and remove blockers
- Monitor team velocity and health

---

### Scrum Master → Project Manager
**What**: Sprint results and team insights

**Handoff includes**:
- Sprint completion metrics
- Blockers encountered and resolved
- Team feedback from retrospective
- Risks identified

**Project Manager will**:
- Update project status reports
- Adjust plans based on velocity
- Escalate unresolved blockers

---

## Best Practices for Effective Handoffs

1. **Be proactive**: Don't wait for the receiving role to ask for information
2. **Be specific**: Provide clear, actionable next steps
3. **Be available**: Make yourself available for questions during transition
4. **Be documented**: Write it down; don't rely on verbal handoffs alone
5. **Be timely**: Notify the receiving role when work is ready, don't let it sit
6. **Verify understanding**: Confirm the receiving role has what they need
7. **Close the loop**: Follow up to ensure handoff was successful

---

## Handoff Tracking

Track handoffs in your project board or issue tracking system:
- Tag the receiving role when handing off
- Move the item to the appropriate workflow column
- Set status to indicate handoff state (e.g., "Waiting for Design", "In QA")
- Update due dates if timeline changes

---

_This template was created to address process gaps identified in [issue #4](https://github.com/igbera/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4) to improve role clarity and handoff accountability._
