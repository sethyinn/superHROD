# Solution Design Skill

This is the second step skill of SuperHROD, used to generate professional OD project proposals after requirements are clear, integrating internal knowledge with external best practices.

## When to Use

Trigger when requirement clarification is complete, the user confirms the requirement summary, and is ready to start designing the project proposal.

## Workflow

### Step 0: Reference Material Learning (Priority)

**Before generating any solution, first learn from the reference materials.**

#### Check Reference Directory

Check if there are reference materials in the following directory:
```
.claude/skills/superhrod/skills/solution-design/reference/
```

#### Read and Analyze Reference Materials

If reference materials exist, read and analyze them **before** proceeding to solution design:

1. **Supported Formats:**
   - **PPT/PPTX** - Presentation slides (use image analysis or text extraction)
   - **Word/DOCX** - Document content (use docx skill to read)
   - **PDF** - PDF documents (use PDF reading capability)
   - **Markdown/MD** - Markdown files
   - **Text/TXT** - Plain text files

2. **Learning Points:**
   - Company's existing OD methodology and framework
   - Previous successful project cases
   - Standard templates and formats
   - Company-specific terminology and language style
   - Constraints and requirements specific to the organization

3. **Integration Principle:**
   - **Priority:** Reference materials > External best practices
   - When conflict exists, follow reference materials first
   - Adapt external best practices to align with reference materials
   - Maintain consistency with company's established approach

4. **If No Reference Materials:**
   - Skip this step
   - Proceed to Step 1 with external best practices only
   - Note: "Consider adding reference materials for more customized solutions"

#### Reference Material Summary (Output)

After learning, generate a brief summary:

```markdown
## Reference Materials Learned

**Materials Found:** [List files read]
**Key Frameworks Identified:** [Frameworks/methodologies from references]
**Company Style:** [Terminology, format, approach preferences]
**Integration Plan:** [How these will be applied to the solution]
```

---

### Step 1: Internal and External Information Collection

#### Internal Knowledge Base Query

Before generating the proposal, query internal resources first:

1. **Historical Projects** - Search for similar historical projects in the project
2. **Best Practice Library** - Query the company's OD best practices
3. **Lessons Learned** - Review lessons learned from past projects

If internal resources are insufficient, mark: "Will supplement with external best practices"

#### External Information Search (via MCP)

Use WebSearch or MCP tools to search for external information, customizing search strategy based on project type:

**General Searches:**
- "[Project Type] best practices 2024"
- "[Project Type] industry cases"
- "[Project Type] implementation guide"

**Targeted Searches:**

| Project Type | Search Keyword Examples |
|---|---|
| Engagement Improvement | "employee engagement improvement project tech company", "Gallup engagement research 2024", "Google Project Oxygen" |
| Org Structure Adjustment | "tech company org structure best practices", "flat organization case", "matrix management pros cons" |
| Performance System | "OKR vs KPI comparison", "tech company performance system case", "360 degree assessment effectiveness" |
| Culture Transformation | "corporate culture change methodology", "Netflix culture handbook", "culture change failure case" |
| Leadership Development | "leadership development program best practices", "hi-po identification criteria", "leadership model" |

**Search Dimensions:**
1. **Research Data** - Research reports from authoritative institutions (Gallup, SHRM, HBR, etc.)
2. **Industry Cases** - Success/failure cases from same industry or benchmark companies
3. **Methodologies** - Industry-recognized methodologies and frameworks
4. **Latest Trends** - Latest trends and practices in 2024
5. **Regulations & Policies** - Relevant laws, regulations, and policy requirements

### Step 2: Integrate Internal and External Perspectives

Compare and analyze internal situations with external information:

1. **Gap Identification** - Gaps between internal practices and external best practices
2. **Feasibility Assessment** - Feasibility of external practices in the company (cost, culture, resources)
3. **Localization Adaptation** - How to adapt external practices to the company's situation
4. **Risk Warnings** - Potential risks of certain external practices

### Step 3: Generate Proposal in Sections

**Important Principle: Present in sections, 200-300 words per section**

Generate the proposal in sections according to the following structure, asking the user if satisfied after each section:

#### Section 1: Problem Diagnosis and Root Cause Analysis

Content Points:
- Diagnosis methods and tools
- Potential root cause hypotheses
- Plans to verify hypotheses

External Reference Markers:
```markdown
**External Research Support:**
- [Research Institution] data shows: [Key Finding]
- [Industry Report] indicates: [Related Conclusion]
```

#### Section 2: Intervention Design

Content Points:
- 2-4 core intervention measures
- Objective, content, implementation method for each measure
- Responsible persons and timeline

External Reference Markers:
```markdown
**Industry Case Reference:**
- [Company Name]'s approach: [Description]
- Success Key: [Key Factor]

**Localization Adaptation:**
- Considerations: [Company's actual situation]
- Adaptation Plan: [Specific adaptations]
```

#### Section 3: Implementation Plan Summary

Content Points:
- Project phase breakdown
- Key milestones
- Resource requirements

#### Section 4: Risks and Responses

Content Points:
- Identify major risks (3-5 items)
- Risk level assessment
- Response measures

External Reference Markers:
```markdown
**Industry Failure Case Warnings:**
- [Case]: [Description] -> Lesson: [Key Lesson]
```

#### Section 5: Effect Evaluation Mechanism

Content Points:
- Evaluation indicators
- Evaluation methods
- Evaluation timing

External Reference Markers:
```markdown
**Industry Evaluation Standards:**
- [Standard/Framework]: [Description]
```

### Step 4: Continue After Each Section Validation

After generating each section, ask the user:
- "Does this part look good?"
- "Do you need any adjustments or additions?"

Proceed to the next section after modifying based on user feedback.

### Step 5: Generate Complete Proposal Document

After all sections are confirmed, integrate into a complete proposal document:

```markdown
# [Project Name] Implementation Plan

## 1. Problem Diagnosis and Root Cause Analysis
[Section 1 Content]

## 2. Intervention Design
[Section 2 Content]

## 3. Implementation Plan Summary
[Section 3 Content]

## 4. Risks and Responses
[Section 4 Content]

## 5. Effect Evaluation Mechanism
[Section 5 Content]

---

## Appendix: Reference Materials

### Internal Materials
- [Historical Project Link]

### External Materials
- [Material 1: Title + Link + Key Points]
- [Material 2: Title + Link + Key Points]
```

## Key Principles

1. **Combine Internal and External** - Internal situation + external wisdom
2. **Present in Sections** - No more than 300 words per section
3. **Continuous Validation** - User confirmation for each section
4. **Cite Sources** - Clearly mark information sources
5. **Localize** - External practices must be adapted to the company

## Output File

After solution design is complete, save to:
`docs/superhrod/solutions/YYYY-MM-DD-<project-name>-solution.md`

## Next Step

After solution design is complete, guide the user to enter the implementation planning phase:
"The proposal has been designed. Next, we can generate a detailed implementation plan. Do you want to continue?"
