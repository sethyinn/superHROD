# Requirement Clarification Skill

This is the first step skill of SuperHROD, used to help clarify project requirements through conversational questioning when HR starts planning OD projects.

## When to Use

Automatically trigger this skill when users mention any HR OD project planning related content:

- "I want to do an engagement improvement project"
- "Need to adjust organizational structure"
- "Need to design a new performance system"
- "How to implement culture transformation"

## Workflow

### Step 1: Understand Project Background

First, identify the basic information of the project:
- **Project Type**: Organization Design / Culture & Engagement / Talent & Performance / Change Management
- **Project Scope**: Which department/group? Company-wide or specific scope?
- **Trigger Reason**: Why do this project now? What's the background?

### Step 2: Collect Information One Question at a Time

**Important Principle: Ask only one question at a time** to avoid information overload.

Collect the following information in order (one question at a time):

1. **Objectives**: What results are expected? How to measure success?
2. **Time Constraints**: Project duration? 3 months/6 months/1 year?
3. **Budget Range**: What's the approximate budget range? Any limitations?
4. **Key Stakeholders**: Who is the project sponsor? Who are the decision makers? Who will be affected?
5. **Team Situation**: How many HR resources? Any external support?
6. **Main Concerns**: What are the biggest risks or concerns?
7. **Success Factors**: What outcomes constitute success?

### Step 3: Generate Requirement Summary

After collecting all information, generate a structured requirement document:

```markdown
## Project Requirement Summary

**Project Type:** [Type]
**Project Name:** [Name]

### Basic Information
- **Scope:** [Department/Group/Size]
- **Objectives:** [Specific expected results]
- **Period:** [Start Time] - [End Time]
- **Budget:** [Budget Range]

### Stakeholders
- **Sponsor:** [Name/Position]
- **Decision Maker:** [Name/Position]
- **Core Team:** [Team Members]

### Constraints
- **Time Constraints:** [Description]
- **Budget Constraints:** [Description]
- **Resource Constraints:** [Description]

### Main Risks and Concerns
- [Risk 1]
- [Risk 2]

### Success Criteria
- [Measurable success criterion 1]
- [Measurable success criterion 2]
```

### Step 4: Confirm and Adjust

Present the requirement summary to the user and ask:
- "Is this information accurate?"
- "Are there any omissions or areas that need modification?"

Adjust based on user feedback until requirements are clear.

## Key Principles

1. **One Question at a Time** - Don't ask multiple questions at once
2. **Follow Up on Details** - When answers are vague, continue to ask
3. **Organize Information** - Organize and summarize information in a timely manner
4. **Confirm Understanding** - Before proceeding to the next step, ensure understanding is correct

## Output File

After requirement clarification is complete, save the requirement summary to:
`docs/superhrod/requirements/YYYY-MM-DD-<project-name>-requirements.md`

## Next Step

After requirement clarification is complete, guide the user to enter the solution design phase:
"Requirements are now clear. Next, we can start designing the project proposal. Do you want to continue?"
