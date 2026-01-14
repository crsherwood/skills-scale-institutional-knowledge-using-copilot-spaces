# OctoAcme — Cross-Role Collaboration and Handoff Guide

## Purpose
This guide provides templates and best practices for effective communication and handoffs between different roles on OctoAcme projects. Clear handoffs reduce rework, improve quality, and ensure accountability.

## When to Use
Reference this guide when coordinating work across roles, especially at key handoff points like requirements to design, design to development, or development to testing.

---

## Key Collaboration Patterns

### 1. Requirements Definition Flow
**Business Analyst → Product Manager → Developers → QA Lead**

#### Business Analyst to Product Manager
**Handoff Artifact**: Requirements Document or User Stories

**Checklist**:
- [ ] Business requirements clearly documented with rationale
- [ ] Stakeholder needs and constraints identified
- [ ] Process flows or workflows diagrammed
- [ ] Business rules and validation logic specified
- [ ] Dependencies on other systems or teams noted

**Communication Template**:
```
Subject: Requirements Ready for Review - [Feature Name]

Hi [Product Manager],

I've completed the requirements analysis for [Feature Name]. Key highlights:

Business Need: [Brief summary]
Stakeholders Consulted: [List]
Key Requirements: [Top 3-5 requirements]
Business Rules: [Critical rules]
Dependencies: [Any dependencies identified]
Open Questions: [Items needing PM input]

Document Link: [Link to requirements doc]
Next Steps: Please review and let's discuss prioritization.
```

#### Product Manager to UX Designer
**Handoff Artifact**: Product Requirements Document with User Stories

**Checklist**:
- [ ] User stories written in "As a [user], I want [goal], so that [benefit]" format
- [ ] Success metrics defined
- [ ] Target users and use cases identified
- [ ] Constraints and trade-offs documented
- [ ] Design principles or brand guidelines shared

**Communication Template**:
```
Subject: Ready for Design - [Feature Name]

Hi [UX Designer],

[Feature Name] is ready for design work. Here's what you need to know:

User Problem: [What problem are we solving?]
Target Users: [Who will use this?]
Success Metrics: [How will we measure success?]
Key User Stories: [Link to stories]
Constraints: [Technical, timeline, or brand constraints]
Inspiration/References: [Any examples or competitive analysis]

Timeline: Design needed by [date] for sprint planning.
Let's sync up to discuss any questions.
```

#### UX Designer to Developers
**Handoff Artifact**: Design Specs, Mockups, Prototypes

**Checklist**:
- [ ] High-fidelity mockups or interactive prototypes provided
- [ ] Design specs annotated with measurements, colors, fonts
- [ ] User flows documented
- [ ] Accessibility requirements specified (WCAG level, screen reader support)
- [ ] Edge cases and error states designed
- [ ] Assets exported in required formats

**Communication Template**:
```
Subject: Design Ready for Development - [Feature Name]

Hi Development Team,

The design for [Feature Name] is complete and ready for implementation.

Design Files: [Link to Figma/Sketch/etc]
Prototype: [Link to interactive prototype]
Accessibility Requirements: [WCAG level, specific considerations]
Key Interactions: [Important UX behaviors to preserve]
Assets: [Link to exported assets/design system components]

Open Items:
- [Any design decisions still in progress]
- [Questions for engineering feasibility]

Please review and flag any implementation concerns. Happy to pair during development.
```

### 2. Development and Testing Flow
**Developers → QA Lead → DevOps Engineer**

#### Developers to QA Lead
**Handoff Artifact**: Completed Feature with Test Build

**Checklist**:
- [ ] Feature meets acceptance criteria
- [ ] Unit tests written and passing
- [ ] Code reviewed and merged
- [ ] Known limitations or edge cases documented
- [ ] Test environment deployed

**Communication Template**:
```
Subject: Ready for QA - [Feature Name]

Hi [QA Lead],

[Feature Name] is deployed to [test environment] and ready for testing.

User Stories Implemented: [Links to stories]
Acceptance Criteria: [Link or brief summary]
Test Account/Data: [Credentials and test data needed]
Known Issues/Limitations: [Anything QA should be aware of]
Areas Needing Extra Attention: [Complex logic, edge cases, integrations]

Please let me know if you need any clarification or find issues to reproduce.
```

#### QA Lead to Developers
**Handoff Artifact**: Test Results and Defect Reports

**Checklist**:
- [ ] Test cases executed and results documented
- [ ] Defects logged with reproduction steps
- [ ] Severity and priority assigned
- [ ] Screenshots or videos attached for visual issues
- [ ] Regression testing scope identified

**Communication Template**:
```
Subject: QA Results - [Feature Name]

Hi Development Team,

Testing for [Feature Name] is complete. Summary:

Test Cases Executed: [Number passed/failed]
Defects Found: [Number and severity breakdown]
Critical Issues: [Link to P0/P1 defects]
Pass Criteria Met: [Yes/No and explanation]

Top Issues Needing Attention:
1. [Issue #123] - [Brief description]
2. [Issue #124] - [Brief description]

Next Steps: [Retest after fixes / Additional testing needed / Ready for staging]
```

#### Developers to DevOps Engineer
**Handoff Artifact**: Release Candidate with Deployment Instructions

**Checklist**:
- [ ] All tests passing in CI
- [ ] Deployment instructions or runbook updated
- [ ] Configuration changes documented
- [ ] Database migrations or schema changes specified
- [ ] Rollback procedure documented
- [ ] Monitoring and alerts configured

**Communication Template**:
```
Subject: Ready for Deployment - [Release Version]

Hi [DevOps Engineer],

[Release Version] is ready for deployment to [staging/production].

Release Tag: [Git tag or build number]
Deployment Runbook: [Link to runbook]
Configuration Changes: [Environment variables, feature flags, etc]
Database Changes: [Migration scripts and rollback steps]
Dependencies: [New services, libraries, or infrastructure needed]
Rollback Plan: [How to roll back if needed]
Monitoring: [Key metrics to watch post-deployment]

Proposed Deployment Window: [Date and time]
Please review and confirm the deployment plan.
```

### 3. Agile Ceremonies and Facilitation
**Scrum Master coordination with all roles**

#### Scrum Master: Sprint Planning Preparation
**Communication Template**:
```
Subject: Sprint Planning Preparation - Sprint [Number]

Team,

Sprint Planning is scheduled for [date/time]. Please prepare:

Product Manager:
- [ ] Backlog refined and prioritized
- [ ] Top stories have clear acceptance criteria
- [ ] Dependencies identified

Developers:
- [ ] Review backlog items
- [ ] Prepare questions or estimation concerns
- [ ] Identify technical risks

QA Lead:
- [ ] Review testing requirements for proposed stories
- [ ] Identify test environment needs

DevOps Engineer:
- [ ] Confirm infrastructure availability
- [ ] Note any planned maintenance windows

Agenda: [Link to planning agenda and backlog]
Let's come prepared for a productive planning session!
```

### 4. Project Status and Reporting
**Project Manager coordination across roles**

#### Project Manager: Weekly Status Update Template
```
Subject: Weekly Status Update - [Project Name] - [Date]

## Progress This Week
- [Key accomplishment 1]
- [Key accomplishment 2]
- [Key accomplishment 3]

## Plan for Next Week
- [Planned work item 1]
- [Planned work item 2]
- [Planned work item 3]

## Metrics
- Velocity: [Current sprint velocity]
- Burndown: [On track / Behind by X points]
- Defect Count: [Open critical/high priority issues]
- Test Coverage: [Percentage]

## Risks and Blockers
| Risk/Blocker | Impact | Owner | Mitigation | Status |
|--------------|--------|-------|------------|--------|
| [Description] | High/Med/Low | [Name] | [Action] | Open/Mitigated |

## Decisions Needed
- [Decision 1] - Need input from [stakeholder] by [date]
- [Decision 2] - Blocker for [work item]

## Kudos
- Shoutout to [team member] for [achievement]

## Questions or Concerns?
Please reach out with any questions or concerns.
```

---

## Role-Specific Communication Guidelines

### Business Analyst
**Best Practices**:
- Always link requirements to business value or user need
- Use visual models (flowcharts, diagrams) to clarify complex workflows
- Document assumptions and constraints explicitly
- Follow up workshops with written summaries for confirmation

### UX Designer
**Best Practices**:
- Provide design rationale, not just mockups
- Make designs accessible (provide text alternatives, consider keyboard navigation)
- Include all states (loading, error, empty, success)
- Partner early with developers on feasibility

### Scrum Master
**Best Practices**:
- Keep ceremonies timeboxed and focused
- Make impediments visible and follow through on removal
- Celebrate small wins and team progress
- Create psychological safety for honest retrospectives

### DevOps Engineer
**Best Practices**:
- Document all infrastructure changes in version control
- Communicate planned maintenance windows early
- Make deployment status visible (dashboards, status pages)
- Provide clear runbooks for common operational tasks

### QA Lead
**Best Practices**:
- Involve QA early in requirements and design phases
- Provide clear reproduction steps for all defects
- Balance manual and automated testing based on risk
- Communicate testing progress and blockers daily

---

## Escalation Paths

### When Collaboration Breaks Down

**Level 1: Peer-to-Peer** (Within 1 day)
- Directly discuss the issue with the other role
- Seek to understand constraints and find compromise
- Document agreements or continued disagreements

**Level 2: Scrum Master or Project Manager** (Within 2 days if unresolved)
- Escalate to Scrum Master for process issues
- Escalate to Project Manager for scope or timeline conflicts
- Provide context and proposed solutions

**Level 3: Product Manager or Management** (For business impact)
- Escalate when business priorities need clarification
- Escalate when technical/design trade-offs affect product goals
- Escalate when risks threaten project success

---

## Tips for Effective Collaboration

1. **Communicate Early and Often**: Don't wait for formal handoffs; involve other roles early for feedback
2. **Assume Positive Intent**: Most issues arise from misunderstanding, not malice
3. **Document Decisions**: Use shared documents, decision logs, or project boards
4. **Close the Loop**: Always confirm receipt and understanding of handoffs
5. **Build Relationships**: Informal conversations build trust that makes formal handoffs smoother
6. **Adapt to Context**: Use lightweight communication for small changes, formal handoffs for complex work
7. **Seek Feedback**: Ask other roles what would make handoffs easier

---

## Feedback and Improvement

This guide is a living document. If you discover better collaboration patterns or templates, please:
- Share them in retrospectives
- Update this document via pull request
- Help onboard others to improved practices

Effective collaboration is a continuous learning process!
