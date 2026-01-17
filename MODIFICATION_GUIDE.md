# SuperHROD Modification Guide

This document helps you understand how to modify and customize the SuperHROD skill.

---

## How to Request Modifications

### Simple Method (Recommended)

Simply tell Claude what you want to change, for example:

- "I want to adjust the order of requirement clarification questions"
- "The external search keywords for solution design need optimization"
- "Add a new module to the PMO table"
- "Modify the workflow of a specific skill"

Claude will automatically locate the corresponding files and help you make the modifications.

### Specific Method

If you know exactly which file you want to modify:

```
"Modify the third step of superhrod/skills/solution-design/SKILL.md"
"Change this content to: [paste new content]"
```

---

## File Structure Overview

```
superhrod/
├── SKILL.md                           # Main entry point - Overall introduction
├── MODIFICATION_GUIDE.md              # This file - Modification guide
├── commands/                          # Command shortcuts
│   ├── clarify-requirements.md
│   ├── design-solution.md
│   ├── create-plan.md
│   └── export-pmo-table.md
├── skills/                            # Core skills (main modification area)
│   ├── requirement-clarification/
│   │   └── SKILL.md                  # Requirement clarification logic
│   ├── solution-design/
│   │   └── SKILL.md                  # Solution design logic + search strategy
│   ├── implementation-planning/
│   │   └── SKILL.md                  # Implementation plan generation logic
│   ├── pmo-table-generator/
│   │   └── SKILL.md                  # PMO table module definitions
│   ├── project-tracking/
│   │   └── SKILL.md                  # Project tracking logic
│   └── knowledge-base/
│       └── best-practices.md         # OD best practices knowledge base
└── examples/
    └── engagement-project.md         # Usage examples
```

---

## Common Modification Scenarios

### 1. Adjusting Requirement Clarification Questions

**File:** `skills/requirement-clarification/SKILL.md`

**Location:** "Step 2: Collect information one question at a time" section

**Example:**
```markdown
Before:
1. Objectives
2. Time constraints
3. Budget range

After:
1. Project objectives
2. Budget range
3. Time constraints
4. Team size
```

### 2. Optimizing External Search Keywords

**File:** `skills/solution-design/SKILL.md`

**Location:** "External Information Search (via MCP)" section

**Example:**
```markdown
Add new search keywords:
| Project Type | Search Keyword Examples |
|---|---|
| Engagement Improvement | "employee engagement tech company 2024", "Gallup engagement research" |
```

### 3. Adding PMO Table Modules

**File:** `skills/pmo-table-generator/SKILL.md`

**Location:** "Step 2: Generate PMO Standard Tables" section

**Example:**
```markdown
Add new module:
#### Module 12: Stakeholder Analysis Table
```markdown
## Stakeholder Analysis Table
| Stakeholder | Interest Level | Influence | Management Strategy |
```

### 4. Expanding Knowledge Base

**File:** `skills/knowledge-base/best-practices.md`

**Location:** Add new content under any section

**Example:**
```markdown
### Engagement Improvement

Add new content:
**Latest Digital Interventions:**
- AI-driven real-time engagement monitoring
- Personalized engagement improvement recommendations
```

### 5. Adjusting Workflow Steps

**File:** SKILL.md of the corresponding skill

**Location:** "Workflow" section

**Example:**
```markdown
Before:
### Step 1: xxx
### Step 2: xxx
### Step 3: xxx

After:
### Step 1: xxx
### Step 2: xxx  # New step
### Step 3: xxx
### Step 4: xxx
```

---

## Modification Recommendations

### Small Modifications
- Adjust question order
- Modify text descriptions
- Add/delete individual fields
→ Just tell Claude directly

### Medium Modifications
- Add new workflow steps
- Add a new PMO table module
- Expand a knowledge base section
→ Tell Claude your specific requirements, Claude will help you modify

### Large Modifications
- Add a new skill module
- Restructure a skill's workflow
→ Recommend discussing requirements clearly first, then modify together

---

## Pre-Modification Recommendations

1. **Backup** - For important modifications, you can ask Claude to backup the original file first
2. **Test** - After modification, it's recommended to test with examples in the examples folder
3. **Record** - You can add a modification record at the end of the file

```markdown
## Modification Record
| Date | Modification Content | Modified By |
|---|---|---|
| 2026-01-17 | Initial version | Claude |
```

---

## Frequently Asked Questions

**Q: What if I'm not sure which file to modify?**
A: Simply describe the functionality you want to change, and Claude will help you locate it.

**Q: What if I make a mistake?**
A: Claude has modification history and can roll back. Or ask Claude to regenerate the original file.

**Q: How can I view the complete content of a specific skill?**
A: Tell Claude "View the content of [skill name]" and it will show you.

**Q: Can I add new skill modules?**
A: Yes, tell Claude what skill you want to add, and it will help you create the file and integrate it.

---

## Contacting Claude

Whenever you need to make modifications, simply tell Claude:

- "I want to modify SuperHROD..."
- "Adjust the xxx..."
- "Add to SuperHROD..."
- "Look at SuperHROD's..."

Claude will understand your intent and help you complete the modifications.

---

**Last Updated:** 2026-01-17
