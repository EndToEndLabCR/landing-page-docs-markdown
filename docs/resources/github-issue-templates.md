# GitHub Issue Templates - EndToEndLabCR Landing Page

## Epic Issue Template

```markdown
---
name: Epic
about: Track a major feature area
title: "[EPIC] "
labels: epic
assignees: ""
---

## Epic Overview

**Epic Name**: [Epic Name]  
**Priority**: [Must Have | Should Have | Could Have]  
**Phase**: [MVP | Phase 1 | Phase 2 | Phase 3]  
**Total Effort**: [X story points]

## Description

[Brief description of what this epic encompasses]

## Goal

[What does success look like for this epic?]

## User Stories

- [ ] #[issue-number] - [Story title]
- [ ] #[issue-number] - [Story title]
- [ ] #[issue-number] - [Story title]

## Acceptance Criteria

- [ ] [High-level acceptance criterion 1]
- [ ] [High-level acceptance criterion 2]
- [ ] [High-level acceptance criterion 3]

## Dependencies

- **Blocks**: [List of epics/stories this blocks]
- **Blocked By**: [List of epics/stories this is blocked by]

## Technical Considerations

[Key technical notes, patterns to follow, architecture decisions]

## Definition of Done

- [ ] All user stories completed
- [ ] All acceptance criteria met
- [ ] Tests passing (> 80% coverage)
- [ ] Documentation updated
- [ ] Code reviewed and merged
- [ ] Deployed to staging
- [ ] Product Owner accepts

## Resources

- Design: [Link to Figma/design files]
- Documentation: [Link to relevant docs]
- API Spec: [Link if applicable]
```

---

## User Story Issue Template

```markdown
---
name: User Story
about: Implement a specific feature or capability
title: ""
labels: user-story
assignees: ""
---

## User Story

**As a** [user type],  
**I want to** [action/goal],  
**So that** [benefit/outcome].

## Epic

Part of: #[epic-issue-number]

## Priority

[Must Have | Should Have | Could Have | Won't Have]

## Acceptance Criteria

- [ ] **Given** [initial context/state]
- [ ] **When** [action/trigger]
- [ ] **Then** [expected result]
- [ ] **And** [additional requirement]

## Technical Notes

- [Implementation detail 1]
- [Implementation detail 2]
- [Security/validation requirement]
- [Performance requirement]

## Tasks

- [ ] [Task description] ([Role], [X SP])
- [ ] [Task description] ([Role], [X SP])
- [ ] [Task description] ([Role], [X SP])

## Dependencies

- **Depends On**: #[issue-number] - [description]
- **Blocks**: #[issue-number] - [description]

## Story Points

**Estimate**: [X story points]

## Definition of Done

- [ ] Code implemented and follows style guide
- [ ] Tests written (unit + integration if applicable)
- [ ] Code reviewed and approved
- [ ] Documentation updated
- [ ] Acceptance criteria verified
- [ ] Deployed to staging
- [ ] Product Owner accepts

## Resources

- Design: [Link to design mockup]
- API Docs: [Link if applicable]
- Reference: [Link to related documentation]
```

---

## Bug Issue Template

```markdown
---
name: Bug Report
about: Report a bug or defect
title: "[BUG] "
labels: bug
assignees: ""
---

## Bug Description

[Clear and concise description of the bug]

## Steps to Reproduce

1. [First step]
2. [Second step]
3. [Third step]

## Expected Behavior

[What should happen]

## Actual Behavior

[What actually happens]

## Environment

- **Browser**: [e.g., Chrome 120, Safari 17]
- **OS**: [e.g., macOS 14, Windows 11]
- **Device**: [e.g., Desktop, iPhone 14]
- **Screen Size**: [e.g., 1920x1080, 375x667]
- **Environment**: [Production | Staging | Local]

## Screenshots/Videos

[If applicable, add screenshots or screen recordings]

## Console Errors
```

[Paste any console errors here]

```

## Severity

[Critical | High | Medium | Low]

## Priority

[Urgent | High | Medium | Low]

## Related Issues

[Link to related issues if any]
```

---

## Technical Debt/Improvement Template

```markdown
---
name: Technical Debt / Improvement
about: Track technical debt or improvement opportunities
title: "[TECH-DEBT] "
labels: tech-debt
assignees: ""
---

## Description

[What needs to be improved or refactored]

## Current Situation

[Describe the current implementation or state]

## Proposed Solution

[Describe the desired end state]

## Benefits

- [Benefit 1]
- [Benefit 2]
- [Benefit 3]

## Effort Estimate

[X story points] - [Estimated time]

## Priority

[High | Medium | Low]

## Risks of Not Addressing

[What happens if we don't fix this?]

## Related Issues

[Link to related issues]
```

---

## Sprint Planning Template

```markdown
# Sprint [Number]: [Sprint Name]

**Duration**: [Start Date] - [End Date]  
**Sprint Goal**: [What is the primary objective of this sprint?]

## Team Capacity

- **Tech Lead**: [X SP]
- **Backend Engineer**: [X SP]
- **Frontend Engineer**: [X SP]
- **UI/UX Engineer**: [X SP]
- **Total Capacity**: [X SP]

## Committed Stories

### High Priority

- [ ] #[issue] - [Story title] ([X SP]) - @assignee

### Medium Priority

- [ ] #[issue] - [Story title] ([X SP]) - @assignee

### Low Priority / Stretch Goals

- [ ] #[issue] - [Story title] ([X SP]) - @assignee

## Dependencies

- [List any external dependencies or blockers]

## Risks

- [Identify any risks to sprint success]

## Notes

[Any additional notes or context for the sprint]
```

---

## Release Checklist Template

```markdown
# Release [Version] Checklist

**Release Date**: [Date]  
**Release Manager**: @[username]  
**Release Type**: [Major | Minor | Patch]

## Pre-Release

### Code

- [ ] All planned features merged to main
- [ ] All tests passing
- [ ] Code freeze announced
- [ ] Version number updated
- [ ] Changelog updated

### Testing

- [ ] Smoke tests completed
- [ ] Regression tests passed
- [ ] Cross-browser testing completed
- [ ] Mobile testing completed
- [ ] Accessibility audit passed
- [ ] Performance benchmarks met
- [ ] Security scan passed

### Documentation

- [ ] User documentation updated
- [ ] API documentation updated
- [ ] Release notes prepared
- [ ] Migration guide (if needed)

### Infrastructure

- [ ] Staging deployment successful
- [ ] Staging smoke tests passed
- [ ] Database migrations tested
- [ ] Rollback plan documented
- [ ] Monitoring and alerts configured

## Release

- [ ] Production deployment initiated
- [ ] Database migrations executed (if any)
- [ ] Production smoke tests passed
- [ ] Monitoring verified
- [ ] Rollback plan ready

## Post-Release

- [ ] Release announcement sent
- [ ] Stakeholders notified
- [ ] Documentation published
- [ ] Release tagged in Git
- [ ] Post-release retrospective scheduled
- [ ] Monitor for 24 hours

## Rollback Plan

[Document steps to rollback if issues arise]

## Known Issues

[List any known issues that are acceptable for this release]
```

---

## Epic Creation Workflow

1. **Create Epic Issue**

   - Use Epic template
   - Add to project board
   - Assign to appropriate phase milestone
   - Add epic label

2. **Break Down into User Stories**

   - Create individual user story issues
   - Reference epic in each story
   - Link stories in epic description

3. **Estimate and Prioritize**

   - Estimate story points for each story
   - Prioritize using MoSCoW method
   - Identify dependencies

4. **Assign to Sprint**

   - Add stories to sprint milestones
   - Assign to team members
   - Track in project board

5. **Track Progress**
   - Update story status as work progresses
   - Check off completed stories in epic
   - Update epic status when complete

---

## GitHub Labels

### Type Labels

- `epic` - Major feature area
- `user-story` - User story implementation
- `bug` - Something isn't working
- `tech-debt` - Technical improvement needed
- `documentation` - Documentation updates

### Priority Labels

- `priority: critical` - Must be done immediately
- `priority: high` - Should be done soon
- `priority: medium` - Normal priority
- `priority: low` - Can be deferred

### Phase Labels

- `phase: mvp` - MVP scope
- `phase: 1` - Phase 1 scope
- `phase: 2` - Phase 2 scope
- `phase: 3` - Phase 3 scope

### Role Labels

- `role: tech-lead` - Tech Lead responsibility
- `role: backend` - Backend Engineer
- `role: frontend` - Frontend Engineer
- `role: ui-ux` - UI/UX Engineer

### Status Labels

- `status: blocked` - Blocked by dependency
- `status: in-progress` - Currently being worked on
- `status: review` - In code review
- `status: testing` - In testing phase
- `status: done` - Completed

---

## Issue Linking Syntax

- Closes #123 - Closes issue when PR merged
- Fixes #123 - Same as closes
- Resolves #123 - Same as closes
- Part of #123 - References without closing
- Blocked by #123 - Indicates dependency
- Blocks #123 - Indicates this blocks another
