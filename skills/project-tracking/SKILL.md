# Project Tracking Skill

This is an execution phase skill for SuperHROD, designed to provide tracking support during project implementation, including progress updates, risk alerts, milestone reviews, and more.

## When to Use

Triggered after project initiation when the user needs to track project progress, manage risk issues, or conduct milestone reviews.

## Workflow

### Step 1: Check Project Status

When the user inquires about project progress or needs tracking, first:

1. **Read PMO Dashboard** - Read the project's PMO dashboard from `docs/superhrod/pmo/`
2. **Check Current Date** - Compare against planned dates to determine if the project is on schedule
3. **Identify Issues** - Check for any delays, risks, or issues requiring attention

### Step 2: Generate Status Report

Based on current project data, generate a status report:

```markdown
## Project Status Report

**Report Date:** [Current Date]
**Reporting Period:** [Last Week/Last Month] - [Current Date]

### Overall Status
🟢 On Track / 🟡 At Risk / 🔴 Critical Issues

### Progress Summary
- **Planned Tasks:** X tasks
- **Completed:** Y tasks
- **In Progress:** Z tasks
- **Delayed:** N tasks
- **Completion Rate:** Y/X %

### Milestone Status
| Milestone | Planned Date | Current Status | Status |
|---|---|---|---|
| M1 Project Kickoff | 3/1 | Completed | ✅ |
| M2 Diagnosis Complete | 3/31 | In Progress | 🔄 |
| M3 Implementation Complete | 5/31 | Not Started | ⏳ |

### Completed Tasks This Period
- [Task 1] - [Completion Date]
- [Task 2] - [Completion Date]

### Upcoming Plans
- [Task 1] - [Planned Date]
- [Task 2] - [Planned Date]

### Risk Monitoring
| Risk | Level | Status |
|---|---|---|
| [Risk Description] | High/Medium/Low | Monitoring/Mitigated/Closed |

### Attention Required
⚠️ **[Alert Item]**
- [Delayed Task Alert]
- [Upcoming Milestone Alert]
- [Risk Escalation Alert]
```

### Step 3: Risk Alerts

System automatically detects and provides alerts:

**Time-Related Alerts:**
- Tasks approaching deadline (within 3 days)
- Overdue tasks
- Milestones approaching but prerequisite tasks incomplete

**Resource-Related Alerts:**
- Budget utilization exceeding 80%
- Human resource investment exceeding plan

**Risk-Related Alerts:**
- High-level risks requiring attention
- Issues unresolved for more than 7 days

**Alert Format:**
```markdown
## ⚠️ Risk Alerts

### Time Alerts
🔴 **Critical Delay:** [Task Name] is X days overdue
🟡 **Approaching Deadline:** [Task Name] due within 3 days

### Resource Alerts
🟡 **Budget Alert:** Training expenses at 85% utilized (42.5k/50k)

### Risk Alerts
🟠 **Risk Escalation:** [Risk Name] requires management attention
```

### Step 4: Provide Adjustment Recommendations

When project deviations occur, provide adjustment recommendations:

```markdown
## Adjustment Recommendations

### Schedule Adjustment
**Issue:** [Task] delayed by 5 days
**Recommended Actions:**
1. [Action 1] - Adjust timeline for subsequent tasks
2. [Action 2] - Increase resource allocation
3. [Action 3] - Reduce task scope

### Risk Response
**Issue:** [Risk] materializing
**Recommended Actions:**
1. [Action 1] - Immediate action
2. [Action 2] - Preventive measures
3. [Action 3] - Contingency plan

### Resource Optimization
**Issue:** [Resource] shortage
**Recommended Actions:**
1. [Action 1] - Reallocate resources
2. [Action 2] - Seek external support
3. [Action 3] - Adjust project scope
```

### Step 5: Milestone Review

Prior to milestone completion, guide user through acceptance:

```markdown
## Milestone Acceptance Review

**Milestone:** [Milestone Name]
**Planned Date:** [Date]

### Acceptance Checklist
- [ ] [Deliverable 1] completed?
- [ ] [Deliverable 2] completed?
- [ ] [Acceptance Criteria] met?
- [ ] [Stakeholder] confirmed?

### Milestone Retrospective
**Achievement Status:** ✅ On Time / 🟡 Delayed X Days / 🔴 Not Achieved

**Lessons Learned:**
- [What went well]
- [Areas for improvement]
- [Optimization opportunities for next time]
```

### Step 6: Update PMO Dashboard

Based on latest progress, update relevant content in the PMO dashboard:
- Update task status
- Update milestone status
- Update risk register
- Update resource utilization
- Document new issues and changes

## User Interaction Modes

### Mode 1: Periodic Status Update

User triggers: "Update project status"

System executes:
1. Read PMO dashboard
2. Ask user which tasks are completed
3. Update task status
4. Generate status report
5. Identify risks and issues

### Mode 2: Risk Consultation

User triggers: "What to do about [risk description]?"

System executes:
1. Assess risk level
2. Provide response recommendations
3. Update risk register

### Mode 3: Milestone Acceptance

User triggers: "Milestone [Name] completed"

System executes:
1. Guide acceptance review
2. Record completion status
3. Facilitate retrospective summary
4. Update milestone status

### Mode 4: Issue Resolution

User triggers: "Encountered issue: [Issue description]"

System executes:
1. Analyze issue impact
2. Provide solution recommendations
3. Update issue log

## Key Principles

1. **Proactive Alerting** - Provide early warnings before issues occur
2. **Data-Driven** - Base analysis on PMO dashboard data
3. **Actionable Recommendations** - Provide specific, executable adjustment recommendations
4. **Closed-Loop Management** - Ensure issues form a closed loop from identification to resolution

## Output Files

Project tracking related documents:
- `docs/superhrod/tracking/YYYY-MM-DD-<project-name>-status-report.md` - Status report
- PMO dashboard automatically updated

## Usage Guidelines

**Recommended Check Frequency:**
- Daily: Check task deadlines
- Weekly: Generate status report, review progress and risks
- Monthly: Comprehensive review of milestones, resource utilization, management reporting
- Milestone checkpoints: Conduct acceptance review and retrospective

## Project Closure

When all milestones are completed, guide project retrospective:

```markdown
## Project Retrospective Summary

**Project Name:** [Name]
**Project Period:** [Start] - [End]
**Report Date:** [Date]

### Project Outcomes
- [Goal achievement status]
- [Key results]
- [Data comparison]

### Success Factors
1. [Factor 1]
2. [Factor 2]

### Lessons Learned
**What Went Well:**
- [Good practice 1]
- [Good practice 2]

**Areas for Improvement:**
- [Issue 1] - [Improvement recommendation]
- [Issue 2] - [Improvement recommendation]

### Knowledge Capture
Update best practices repository:
- [Reusable practices]
- [Pitfalls to avoid]

### Next Steps
- [Follow-up work]
- [Continuous improvement recommendations]
```

Upon completion of project retrospective, save to:
`docs/superhrod/reviews/YYYY-MM-DD-<project-name>-review.md`
