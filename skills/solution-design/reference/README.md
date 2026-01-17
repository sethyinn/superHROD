# Solution Design Reference Materials

This directory stores reference materials for the Solution Design skill. Claude will learn from these materials before generating any OD project solutions.

## Purpose

Reference materials help Claude:
- Understand your company's existing OD methodology
- Learn from your previous successful projects
- Follow your standard templates and formats
- Use company-specific terminology and language style
- Align with your organizational constraints and requirements

## Supported File Types

| Format | Description | Usage |
|--------|-------------|-------|
| **PPT/PPTX** | Presentation slides | Methodology frameworks, training materials |
| **Word/DOCX** | Word documents | Project proposals, case studies, templates |
| **PDF** | PDF files | Research reports, best practice guides |
| **Markdown/MD** | Markdown files | Documentation, process guides |
| **Text/TXT** | Plain text | Quick reference notes |

## How to Use

1. **Place reference materials in this directory**
   - Copy your PPT, Word, PDF, or other files here
   - Files will be automatically read before solution design

2. **Organize by category (optional)**
   ```
   reference/
   ├── methodologies/          # OD frameworks and methodologies
   ├── cases/                 # Previous successful cases
   ├── templates/             # Standard templates
   └── guidelines/            # Company guidelines
   ```

3. **Claude will automatically:**
   - Check this directory when starting solution design
   - Read all available materials
   - Apply learnings to the generated solution
   - Reference materials > External best practices

## Example Reference Materials

### Recommended Content

- **Methodology Documents**
  - Company OD framework
  - Diagnostic tools and approaches
  - Intervention design principles

- **Previous Cases**
  - Successful project proposals
  - Lessons learned documents
  - Case study presentations

- **Templates**
  - Solution design template
  - Standard deliverable formats
  - Report structure examples

- **Guidelines**
  - Company-specific constraints
  - Brand and language guidelines
  - Approval process requirements

## Priority Rules

When generating solutions, Claude follows this priority:

1. **Reference Materials** (Highest priority)
2. **Internal Knowledge Base** (Company best practices)
3. **External Best Practices** (Industry standards)

If reference materials conflict with external practices, reference materials take precedence.

## Tips

- Start with 3-5 key reference materials
- Update materials when your methodology evolves
- Remove outdated materials to avoid confusion
- Use clear file names for easy identification

---

**Last Updated:** 2026-01-17
