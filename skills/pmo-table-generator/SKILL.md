# PMO Table Generation Skill

This is the fourth step skill of SuperHROD, used to generate PMO-standard project management tables after the implementation plan is completed.

## When to Use

Triggered when the user needs to generate PMO-standard project management tables after the implementation plan has been generated.

## Workflow

### Step 1: Collect Implementation Plan Information

Extract the following information from the implementation plan document:
- WBS (Work Breakdown Structure) task decomposition
- Task dependencies
- Timeline planning
- Responsibility assignment matrix
- Milestone plan
- Resource planning

### Step 2: Generate PMO Standard Tables

Generate the following modules according to PMO standards:

#### Module 1: Project Overview Table

```markdown
## Project Overview

| Field | Content |
|---|---|
| **Project Name** | [Project Name] |
| **Project Number** | [Auto-generated: YYYY-Project Type-Sequence] |
| **Project Manager** | [Name] |
| **Project Sponsor** | [Name] |
| **Project Objectives** | [Objective Description] |
| **Start Date** | [Date] |
| **End Date** | [Date] |
| **Project Duration** | [X months] |
| **Total Budget** | [Amount] |
| **Current Status** | Planning/In Progress/Completed |
```

#### Module 2: WBS Task Decomposition Table

```markdown
## WBS Task Decomposition

| Level 1 Task | Level 2 Task | Level 3 Task | Task Description | Duration | Predecessors | Owner | Status |
|---|---|---|---|---|---|---|---|
| 1.Preparation Phase | 1.1 Project Initiation | 1.1.1 Team Formation | Form project team | 2h | - | Zhang San | Not Started |
```

#### Module 3: Milestone Plan Table

```markdown
## Milestone Plan

| Milestone ID | Milestone Name | Deliverables | Acceptance Criteria | Planned Date | Actual Date | Status |
|---|---|---|---|---|---|---|
| M1 | Project Initiation | Project Charter | Signature Obtained | 3/1 | - | Not Started |
```

#### Module 4: Responsibility Assignment Matrix (RACIC)

```markdown
## Responsibility Assignment Matrix (RACIC)

| Task | Role A | Role B | Role C | Role D |
|---|---|---|---|---|
| **Role Definition** | HR BP | Department Head | HRD | External Consultant |
| 1.1.1 Team Formation | R | C | A | I |
| 1.1.2 Kickoff Meeting | R | C | A | I |

**Legend:**
- R (Responsible) - Executes the work
- A (Accountable) - Ultimate ownership and decision-making authority
- C (Consulted) - Needs to be consulted
- I (Informed) - Needs to be informed
- C (Checked) - Reviews and accepts deliverables
```

#### Module 5: Gantt Chart Data

```markdown
## Gantt Chart Data

| Task ID | Task Name | Start Date | End Date | Duration | Predecessors |
|---|---|---|---|---|---|
| 1.1.1 | Team Formation | 3/1 | 3/1 | 1d | - |
| 1.1.2 | Kickoff Meeting | 3/2 | 3/2 | 1d | 1.1.1 |
```

#### Module 6: Risk Register

```markdown
## Risk Register

| Risk ID | Risk Description | Impact | Probability | Risk Level | Mitigation Strategy | Owner | Status |
|---|---|---|---|---|---|---|---|
| R1 | Low employee engagement | High | Medium | High | Increase communication, leadership endorsement | HR BP | Monitoring |
| R2 | Budget overrun | Medium | Low | Medium | Strict expense control | Project Manager | Monitoring |

**Impact:** High/Medium/Low
**Probability:** High/Medium/Low
**Risk Level:** High (High×High, High×Medium) / Medium (Medium×Medium, High×Low) / Low (Others)
```

#### Module 7: Communication Plan

```markdown
## Communication Plan

| Stakeholder | Communication Content | Frequency | Method | Owner |
|---|---|---|---|---|
| Management | Project Progress | Monthly | Reporting Meeting | Project Manager |
| Employees | Project Information | Weekly | Email + Intranet | HR BP |
```

#### Module 8: Change Management Table

```markdown
## Change Management

| Change ID | Change Description | Requester | Request Date | Impact Assessment | Approver | Approval Status | Implementation Status |
|---|---|---|---|---|---|---|---|
| CR1 | Extend research period by 1 week | Li Si | 3/15 | Budget +5k, Duration +1 week | HRD | Approved | Implemented |
```

#### Module 9: Issue Log

```markdown
## Issue Log

| Issue ID | Issue Description | Severity | Reported Date | Owner | Status | Resolution |
|---|---|---|---|---|---|---|
| I1 | Survey system malfunction | High | 3/10 | IT Support | Resolved | System replaced |
```

#### Module 10: Resource Utilization Table

```markdown
## Resource Utilization

### Human Resource Investment
| Role | Planned Investment | Actual Investment | Completion Percentage |
|---|---|---|---|
| HR BP | 40h | 20h | 50% |

### Budget Utilization
| Category | Budget | Used | Remaining | Utilization Rate |
|---|---|---|---|---|
| Training Expenses | 50k | 0 | 50k | 0% |
| **Total** | **135k** | **10k** | **125k** | **7.4%** |
```

#### Module 11: Status Report Template

```markdown
## Project Status Report (Period: Weekly/Monthly)

**Reporting Period:** [Start Date] - [End Date]
**Report Date:** [Date]
**Reporter:** [Name]

### Overall Status
🟢 On Track / 🟡 At Risk / 🔴 Critical Issues

### Current Period Progress
- [Completed tasks]
- [Milestones achieved]

### Next Period Plan
- [Tasks planned for completion]
- [Milestones planned for achievement]

### Risks and Issues
| Risk/Issue | Status | Mitigation Actions |
|---|---|---|
| [Description] | [Status] | [Actions]

### Support Required
- [Items requiring decisions]
- [Items requiring resources]
```

### Step 3: Integrate into Complete PMO Table Document

```markdown
# [Project Name] PMO Project Management Tables

**Generation Date:** [Date]
**Version:** 1.0

---

## 1. Project Overview
[Project Overview Table]

## 2. WBS Task Decomposition
[WBS Task Decomposition Table]

## 3. Milestone Plan
[Milestone Plan Table]

## 4. Responsibility Assignment Matrix
[RACIC Matrix]

## 5. Gantt Chart Data
[Gantt Chart Data Table]

## 6. Risk Register
[Risk Register]

## 7. Communication Plan
[Communication Plan Table]

## 8. Change Management
[Change Management Table]

## 9. Issue Log
[Issue Log Table]

## 10. Resource Utilization
[Resource Utilization Table]

## 11. Status Report Template
[Status Report Template]

---

## Appendix

### Change Log
| Version | Change Date | Changed By | Change Description |
|---|---|---|---|
| 1.0 | [Date] | [Name] | Initial version |
```

## Output Format

**Markdown Format** (Default):
- Facilitates version control
- Enables collaborative editing
- Saved in project documentation

**Can Be Exported to Excel**:
- Convert using table tools
- Facilitates PMO reporting
- Enables data visualization

## Key Principles

1. **Completeness** - Include all standard modules required by PMO
2. **Maintainability** - Easy to update and track
3. **Readability** - Clear table formatting
4. **Actionability** - Each table has a clear purpose

## Output File

After PMO tables are generated, save to:
`docs/superhrod/pmo/YYYY-MM-DD-<project-name>-pmo-table.md`

## Usage Guidelines

**Update Frequency:**
- Project overview, WBS, milestones: Established at project initiation, updated for significant changes
- Risk register, issue log: Updated weekly
- Resource utilization: Updated monthly
- Status reports: Generated weekly/monthly

## Next Steps

After PMO tables are generated, prompt the user:
"PMO project management tables have been generated. You can now begin project execution. Do you need execution tracking support?"
