# Implementation Planning Skill

This is the third step skill of SuperHROD, used to break down the approved solution into a detailed, actionable implementation plan.

## When to Use

Triggered after solution design is completed and confirmed by the client, when preparing to generate the specific implementation plan.

## Workflow

### Step 1: Work Breakdown Structure (WBS)

Break down the project into manageable small tasks:

**WBS Hierarchy:**
- **Level 1 Tasks** - Project phases (e.g., Preparation Phase, Diagnosis Phase, Implementation Phase, Evaluation Phase)
- **Level 2 Tasks** - Major work packages (e.g., Design questionnaire, Collect data, Analyze data)
- **Level 3 Tasks** - Specific tasks (e.g., Draft questionnaire design, Internal review, Finalize revisions)

**Task Granularity:**
- Each task estimated to take 2-5 hours to complete
- Tasks have clear start and end markers
- Tasks have verifiable deliverables

**Example:**
```markdown
## WBS Task Breakdown

### 1. Preparation Phase
#### 1.1 Project Initiation
- 1.1.1 Assemble project team [2h]
- 1.1.2 Conduct kickoff meeting [2h]
- 1.1.3 Develop detailed plan [4h]

#### 1.2 Diagnostic Tool Preparation
- 1.2.1 Design questionnaire draft [4h]
- 1.2.2 Internal review of questionnaire [2h]
- 1.2.3 Revise and finalize [2h]
```

### Step 2: Identify Task Dependencies

Mark dependencies between tasks:

- **FS (Finish-to-Start)** - Predecessor task must finish before successor can start
- **SS (Start-to-Start)** - Predecessor task must start before successor can start
- **FF (Finish-to-Finish)** - Predecessor task must finish before successor can finish

**Example:**
```markdown
## Task Dependencies
- 1.2.1 → 1.2.2 (FS): Questionnaire design must be completed before review
- 1.2.2 → 1.2.3 (FS): Review must be completed before revisions
- 2.1.1 and 2.1.2 can run in parallel (SS)
```

### Step 3: Schedule Planning

Estimate duration for each task:

**Estimation Methods:**
- Reference similar historical projects
- Consider resource availability
- Include buffer time (typically 10-20%)

**Output Format:**
```markdown
## Schedule Planning

| Task | Duration | Start Date | End Date |
|---|---|---|---|
| 1.1.1 Assemble project team | 2h | 3/1 | 3/1 |
| 1.1.2 Conduct kickoff meeting | 2h | 3/2 | 3/2 |
```

### Step 4: Responsibility Assignment (RACIC Matrix)

Assign responsibility roles for each task:

**RACIC Definitions:**
- **R (Responsible)** - Person who performs the task
- **A (Accountable)** - Person accountable for task outcomes (only one)
- **C (Consulted)** - People who need to be consulted
- **I (Informed)** - People who need to be informed
- **C (Checked)** - People who check/validate

**Example:**
```markdown
## Responsibility Assignment Matrix (RACIC)

| Task | HR BP | Department Head | HRD | External Consultant |
|---|---|---|---|---|
| 1.1.1 Assemble project team | R | C | A | I |
| 1.1.2 Conduct kickoff meeting | R | C | A | I |
```

### Step 5: Milestone Planning

Define key milestones and acceptance criteria:

```markdown
## Key Milestones

| Milestone | Deliverables | Acceptance Criteria | Timeline |
|---|---|---|---|
| M1: Project Initiation | Project Charter | Stakeholder sign-off obtained | End of Week 1 |
| M2: Diagnosis Complete | Diagnostic Report | Report passes management review | End of Week 4 |
```

### Step 6: Resource Planning

Estimate required resources:

**Human Resources:**
- Time commitment for each role
- External support requirements

**Budget Resources:**
- Survey tool costs
- Training expenses
- Consulting fees
- Other expenses

**Example:**
```markdown
## Resource Planning

### Human Resources
- HR BP: 40 hours
- Department Head: 20 hours
- External Consultant: 60 hours

### Budget
- Survey Tool: 5,000 yuan
- Training Expenses: 50,000 yuan
- Consulting Fees: 80,000 yuan
- **Total: 135,000 yuan**
```

### Step 7: Generate Complete Implementation Plan

Integrate the above content to generate a comprehensive implementation plan document:

```markdown
# [Project Name] Implementation Plan

## 1. WBS Task Breakdown
[Task list]

## 2. Task Dependencies
[Dependencies]

## 3. Schedule Planning
[Timeline]

## 4. Responsibility Assignment Matrix
[RACIC Matrix]

## 5. Milestone Plan
[Milestones]

## 6. Resource Planning
[Resource requirements]

## 7. Critical Path Analysis
[Identify tasks on critical path]

## 8. Risk Alerts
[Risks that may impact schedule]
```

## Key Principles

1. **Actionable Tasks** - Each task should be specific and executable
2. **Clear Accountability** - Each task has a clearly designated owner
3. **Clear Dependencies** - Relationships between tasks are clear and explicit
4. **Trackable** - Each task has clear completion criteria
5. **Buffer Included** - Consider uncertainty and include buffer time

## Output File

After implementation plan is completed, save to:
`docs/superhrod/plans/YYYY-MM-DD-<project-name>-implementation-plan.md`

## Next Step

After implementation plan is generated, guide user to PMO spreadsheet generation phase:
"The implementation plan has been generated. Next, we can generate PMO standard project management spreadsheets. Would you like to continue?"
