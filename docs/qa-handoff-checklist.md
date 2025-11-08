# QA Handoff Checklist

## Purpose
This checklist ensures smooth handoffs between Developers and QA Lead, reducing back-and-forth and ensuring comprehensive testing.

## When to Use
Use this checklist whenever a feature or bug fix is ready for QA validation.

---

## Developer Checklist (Before Handoff to QA)

### Code Quality
- [ ] All automated tests pass (unit, integration, e2e)
- [ ] Code reviewed and approved by at least one peer
- [ ] Linting and code quality checks pass
- [ ] Security scans completed with no critical issues
- [ ] No merge conflicts with target branch

### Documentation
- [ ] Acceptance criteria clearly documented in the issue/story
- [ ] PR description includes summary of changes and testing approach
- [ ] Any new configuration or environment setup documented
- [ ] Screenshots or recordings provided for UI changes

### Test Preparation
- [ ] Test data requirements identified and documented
- [ ] Edge cases and potential failure scenarios listed
- [ ] Dependencies on other features or services noted
- [ ] Rollback plan documented (if applicable)

### Communication
- [ ] Issue/story moved to "QA" column on project board
- [ ] QA Lead tagged/notified with handoff details
- [ ] Testing environment confirmed available and accessible
- [ ] Expected completion date communicated

---

## QA Lead Checklist (During Testing)

### Test Execution
- [ ] Verify all acceptance criteria are met
- [ ] Execute documented test cases
- [ ] Test edge cases and error scenarios
- [ ] Validate UI/UX against design specs (with UX Designer if needed)
- [ ] Test on all supported platforms/browsers (if applicable)
- [ ] Verify performance within acceptable limits

### Regression Testing
- [ ] Confirm related features still work as expected
- [ ] Check for unintended side effects
- [ ] Validate integrations with dependent systems

### Documentation Review
- [ ] Release notes updated (if applicable)
- [ ] User documentation or help text accurate
- [ ] API documentation updated (if applicable)

### Issue Tracking
- [ ] Log any defects found with clear reproduction steps
- [ ] Link bugs to original feature issue
- [ ] Assess severity and priority of issues
- [ ] Communicate blockers to Scrum Master and Project Manager

---

## QA Signoff Decision

### Pass Criteria
Feature is approved when:
- All acceptance criteria validated
- No critical or high-priority bugs remaining
- Regression tests passed
- Performance acceptable
- Documentation complete

**Action**: Move issue to "Done", add QA approval comment

### Fail/Block Criteria
Feature is rejected when:
- Acceptance criteria not met
- Critical bugs found
- Major regressions introduced
- Performance degradation

**Action**: Move issue back to "In Progress", link blocking bugs, notify Developer and Scrum Master

---

## Communication Templates

### Handoff to QA (Developer)
```
@qa-lead Feature XYZ is ready for QA testing.

**What changed**: [Brief summary]
**Testing focus**: [Key areas to validate]
**Test data**: [Instructions or links]
**Edge cases**: [Scenarios to verify]
**Environment**: [Staging URL or setup notes]

Issue: #123
PR: #456
```

### QA Approval (QA Lead)
```
✅ QA Approved

**Tested on**: [environments/browsers]
**Test cases executed**: [number or reference]
**Notes**: [any observations or minor issues]

Ready for release.
```

### QA Rejection (QA Lead)
```
❌ QA Issues Found

**Blocking bugs**: #789, #790
**Severity**: Critical
**Impact**: [description]
**Recommended action**: [fix priority, timeline]

Moving back to In Progress.
```

---

_This checklist was created to address process gaps identified in [issue #4](https://github.com/igbera/skills-scale-institutional-knowledge-using-copilot-spaces/issues/4)._
