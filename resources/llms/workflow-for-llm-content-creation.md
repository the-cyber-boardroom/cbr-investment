# LLM Documentation Framework: Workflow and Style Guide

## Overview
This framework defines the systematic process and standards for creating high-quality documentation using Large Language Models (LLMs). It combines a proven workflow for content development with strict style guidelines to ensure consistency, accuracy, and fidelity to source materials.

## Purpose
This document serves two critical functions:
1. Outlines the parallel LLM workflow for efficient document creation, with specific timing and validation criteria
2. Establishes comprehensive style guidelines ensuring content remains faithful to source materials while maintaining clarity and depth

The framework enables teams to leverage LLMs effectively while ensuring all content maintains direct lineage to authoritative sources. This approach combines the efficiency of AI-assisted writing with the rigor of traditional documentation standards.

## Version Control
- Maintain clear document versioning (v0.1, v0.2, etc.)
- Track major revisions in document header
- Document feedback iterations with timestamps
- Preserve key versions for reference

## Initial Content Generation
### Phase 1: Audio Transcription
1. Author records audio stream-of-consciousness
2. GenAI transcribes audio to text
3. Quick review for transcription accuracy 
4. Output: Raw transcript containing core ideas and concepts
5. Validation: Ensure all key concepts are captured accurately

### Phase 2: Document Structure
1. LLM processes transcript to create structured outline
2. Focus on coherent flow and logical organization
3. Output: Initial document with clear sections and hierarchy

### Phase 3: Content Review
1. Compare structured document against original transcript
2. Identify missing core ideas or concepts
3. Output: Validated document structure with complete coverage

## Parallel LLM Processing
### Browser/LLM #1: Strategic Direction
**Purpose**: Create detailed briefing for content refinement

**Example Briefing Format**:
```markdown
SECTION: [Specific section name]
LOCATION: [Paragraph/line reference]
CURRENT STATE: [Brief description of existing content]
REQUIRED CHANGES:
- Remove: [Specific text to eliminate]
- Add: [New concepts to incorporate]
- Modify: [Content to rework]
RATIONALE: [Explanation for changes]
SUCCESS CRITERIA: [Measurable outcomes]
```

**Process**:
1. Review existing document and creation guidelines
2. Analyze for content duplication
3. Create actionable briefing for Browser/LLM #2
4. Focus on content reduction and simplification
5. Provide specific instructions for text location/modification
6. Iterate with author feedback
7. Always provide answer in a new artifact that can be easily copy and pasted
8. Don't ask to proceed with specific content recommendations for any of these changes, since that will be done in the other section
9. Add note to the Content editing LLM to really focus on the content creation guidlines (specially around the use of dangling bullet points)

**Key Objectives**:
- Eliminate redundant content
- Maintain focus and clarity
- Simplify consumption
- Preserve core message

### Browser/LLM #2: Content Execution
**Purpose**: Implement refinements based on LLM #1 briefing

**Process**:
1. Review current document version
2. Execute briefing instructions from LLM #1
3. Self-evaluate against briefing requirements
4. Incorporate author feedback
5. Refine based on direction
6. Only work on the content defined in the brief
7. Really pay attention to the content creation guidelines
8. Always use a new Artifact for proposed changes
8. After making the changes, back in the main chat window create a table with a rating on how effective the proposed answers and content-changes were against the original brief

## Quality Control
### Output Reconciliation
1. When LLMs produce divergent outputs:
   - Compare against original briefing requirements
   - Identify stronger elements from each version
   - Create consolidated version incorporating best elements
   - Validate against initial objectives

### Optional Verification
1. LLM #1 reviews LLM #2 output
2. Evaluates against original briefing
3. Rates for:
   - Accuracy
   - Quality
   - Completeness

## Success Criteria
- No content duplication
- Clear, focused messaging
- Simple consumption format
- Alignment with author vision
- Comprehensive coverage of core ideas


# Content Creation Style Guide

## Core Principles

* **Document-Based Content** - All content must be derived directly from the provided source documents. Do not introduce external concepts, examples, or ideas that aren't present in the original materials. This ensures consistency and maintains the integrity of the original content's intent.

* **Source Fidelity** - When expanding on ideas, use only the concepts, examples, and frameworks presented in the source documents. While the organization and presentation may be enhanced, the underlying content should remain faithful to the original material.

* **Content Boundaries** - Stay within the conceptual boundaries established by the source documents. While you may restructure and clarify the presentation, avoid introducing new theories or expanding beyond the scope of the provided materials.

* **Evidence-Based Writing** - Every point made should be traceable back to specific content in the source documents. This creates a clear chain of provenance for ideas and ensures the final content remains true to the original material.

## Structure

### Section Organization

* **Context Alignment** - Begin each major section with a context-setting paragraph that draws directly from the themes and concepts present in the source documents. Ensure this context accurately reflects the original material's scope and intent.

* **Hierarchical Clarity** - Use clear hierarchical headings (H2 for main sections, H3 for subsections) to organize content, maintaining the relationship structure found in the source documents.

* **Categorical Consistency** - Group related concepts into distinct categories based on their presentation in the original materials. Don't create new categories that aren't supported by the source content.

* **Forward References** - When concluding sections, focus on implications and forward-looking statements that are explicitly mentioned or clearly implied in the source documents.

### Content Formatting

* **Bullet Point Structure** - Each bullet point should begin with a bold title that captures the key concept, followed by a detailed paragraph that expands on and explains that concept. Single-word or short-phrase bullet points should be avoided as they lack necessary context and depth.

* **Hierarchical Organization** - When nesting bullet points, maintain the same detailed structure at each level. Each sub-point should follow the same format of bold title followed by explanatory paragraph, ensuring consistent depth of information throughout the hierarchy.

* **Categorical Headers** - Include descriptive headers for groups of bullet points to provide context and organization. These headers should clearly indicate the theme or category of the detailed points that follow.

* **Consistency in Detail** - Every bullet point should maintain a similar level of detail and explanation. Avoid mixing detailed bullet points with brief ones, as this creates an uneven reading experience and leaves gaps in understanding.

## Writing Style

### Tone and Approach
* Professional but accessible
* Technical without being overly complex
* Analytical and systematic
* Solutions-oriented
* Forward-thinking

### Paragraph Structure
* Open with context and significance
* Build logical connections between ideas
* Keep paragraphs focused and concise
* End with implications or transitions

### Language Use
* Clear and precise terminology
* Technical terms introduced with context
* Consistent use of industry-standard terms
* Balanced mix of abstract and concrete concepts

## Content Development

### Organization Method
* Start with high-level outline
* Break complex topics into distinct categories
* Build depth through hierarchical structure
* Connect related concepts across sections
* End with practical implications

### Examples and Evidence
* Use real-world examples to illustrate concepts
* Include practical applications
* Reference industry practices
* Connect theoretical frameworks to implementation

## Quality Standards

### Clarity Checks

* **Bullet Point Completeness** - Each bullet point must function as a self-contained unit of information, with a clear bold title followed by a paragraph that fully explains the concept. The explanation should provide enough context that it can be understood even if read in isolation.

* **Logical Flow** - Sections should progress in a natural sequence, with each topic building upon previous information. Transitions between sections should be smooth and logical, helping readers follow the progression of ideas.

* **Terminology Consistency** - Technical terms should be used consistently throughout the document, with clear definitions provided upon first use. The same concept should be referred to by the same term throughout to avoid confusion.

* **Category Organization** - Categories should be structured to be mutually exclusive and collectively exhaustive, ensuring comprehensive coverage without overlap. Each category should have a clear scope and purpose within the larger document structure.

### Structural Integrity

* **Header Level Preservation** - When modifying or adding content to an existing document, maintain the exact header level structure of the surrounding content. If a section uses `##` for main headers and `###` for subsections, new content must follow the same pattern. This ensures consistent document hierarchy and prevents formatting issues during content integration.

* **Indentation Consistency** - All new content must match the indentation patterns of the existing document structure. This includes:
  - Preserving blank lines before and after headers
  - Maintaining consistent list indentation levels
  - Following existing code block formatting
  - Matching bullet point and numbered list styles

* **Section Integration** - When adding new sections:
  - Analyze the existing header structure (e.g., H1 → H2 → H3)
  - Match the header level of peer sections
  - Maintain consistent spacing between sections
  - Preserve any existing section numbering schemes

* **Version Control Compatibility** - Ensure new content follows existing markdown formatting to maintain compatibility with version control systems and documentation tools. This includes:
  - Consistent line breaks between sections
  - Standard markdown syntax for emphasis and formatting
  - Proper nesting of lists and subheaders
  - Compatible link and reference formatting

### Depth Requirements
* Main concepts require thorough explanation
* Supporting points need clear connection to main ideas
* Examples should illustrate practical application
* Implications should be clearly stated


# Interactive LLM Workflow Prompts

## Initial Document Creation
```markdown
We are following the workflow defined in "LLM Documentation Framework: Workflow and Style Guide". I'll be working with you in Phase 2 (Initial Document Creation) where your role is to create a structured document from a transcript.

Please review this audio transcript carefully, focusing on:
- Core ideas and concepts
- Natural structural organization
- Logical flow of information
- Key themes and patterns

[PASTE TRANSCRIPT]

Please create an initial document structure with clear sections and hierarchy. Use descriptive headers and maintain the source material's intent and scope.

```

## Browser/LLM #1 (Strategic Direction)
```markdown
We are following the workflow defined in "LLM Documentation Framework: Workflow and Style Guide". I'll be working with you in Phase 5 (Strategic Direction) where your role is to analyze content and create focused improvement briefings.

First, please review this document carefully, focusing on:
- Identifying content duplication
- Sections where content is already well-covered elsewhere
- Areas that could be simplified or consolidated
- Opportunities for better content organization

[ATTACHED]

Once you've completed your review, I'll share specific sections for improvement, and you'll create detailed briefings following our standard format:

SECTION: [section name]
LOCATION: [paragraph reference]
CURRENT STATE: [content description]
REQUIRED CHANGES:
- Remove: [specific text]
- Add: [new concepts]
- Modify: [content to rework]
RATIONALE: [explanation]
SUCCESS CRITERIA: [measurable outcomes]

Please confirm when you've completed your review and are ready to work on specific sections.
```

## Browser/LLM #2 (Content Execution)
```markdown
We are following the workflow defined in "LLM Documentation Framework: Workflow and Style Guide". I'll be working with you in Phase 6 (Content Execution) where your role is to implement improvement briefings and evaluate the results.

I'll provide:
1. The section to modify
2. A detailed briefing specifying required changes

Please implement the changes precisely as specified and then self-evaluate your work against the success criteria.

Are you ready to begin?
```

## Quality Review (Optional)
```markdown
We are following the workflow defined in "LLM Documentation Framework: Workflow and Style Guide". I'll be working with you in Phase 7 (Quality Review) where your role is to evaluate revised content against original briefing requirements.

I'll provide:
1. Original briefing
2. Revised content

Please analyze alignment, quality, and completeness. Rate each aspect 1-10 with specific feedback.

Are you ready to begin?
```