# SuperHROD - Super HR OD Consultant

SuperHROD is an AI-powered intelligent planning assistant for Organization Development (OD) projects, enabling every HR professional to have professional OD consultant support.

## When to Use

Automatically activate SuperHROD skills when users are planning or implementing HR OD (Organization Development) projects, including:

- **Organization Diagnosis & Design** - Organizational structure adjustment, department restructuring, reporting relationship optimization
- **Culture & Engagement** - Employee engagement improvement, culture transformation projects, leadership development
- **Talent & Performance** - Performance system design, compensation structure optimization, talent review
- **Change Management** - Change management processes, process optimization, digital transformation

## Core Workflow

SuperHROD provides a complete OD project planning workflow:

### 1. Requirement Clarification
Help HR clarify project objectives, scope, constraints, and stakeholders through conversational questioning.

### 2. Solution Design
Generate professional OD project proposals based on requirements, integrating internal knowledge with external best practices.

### 3. Implementation Planning
Break down the solution into executable tasks with clear responsibilities and timelines.

### 4. PMO Table Generation
Generate standard project management tables (WBS, RACIC, risk register, etc.).

### 5. Execution Tracking
Provide project progress tracking and risk alert mechanisms.

## How to Use

### Direct Command Invocation
```
/superhrod:clarify    # Start requirement clarification
/superhrod:design     # Start solution design
/superhrod:plan       # Generate implementation plan
/superhrod:pmo        # Export PMO tables
```

### Automatic Triggering
When Claude Code detects users discussing HR OD project planning, it automatically loads relevant skills.

## Sub-skills

- **requirement-clarification** - Requirement clarification skill
- **solution-design** - Solution design skill (with external search)
- **implementation-planning** - Implementation plan generation skill
- **pmo-table-generator** - PMO table generation skill
- **project-tracking** - Project tracking skill

## Knowledge Base

- **best-practices** - OD best practices
- **case-studies** - Industry case library
- **risk-database** - Risk database

## Relationship with Superpowers

SuperHROD is an extension of Superpowers in the HR OD domain:
- **Superpowers** provides generic software engineering workflows
- **SuperHROD** provides professional knowledge and workflows for HR OD

Both can coexist, and Claude Code will select the appropriate skill set based on task type.

## Design Document

Complete design document: `docs/plans/2026-01-17-superhr-od-advisor-design.md`
