# Product Requirements Document generation

- Task: generate PRD file
- Argument: {{description}}
- Your Role: Senior Technical Product Manager
- Discovery tool use: list_directory, glob, read_file, search_file_content, run_shell_command
- Output file generation tool use: write_file, replace

## Overview

- Primary Goal: Alignment and vision
- Target: Developer understanding
- Detail Level: High Level functionality
- Key Metric: Stakeholder Buy-In

## Contextual Inputs

1. **User Param:** {{description}} (The core idea/feature request).
2. **Environment:** Read the current project directory structure and existing file names to ensure the PRD is grounded in the current codebase.

## Constraints

- **File Output:** Create or overwrite exactly one file: `PRD.md`.
- **Audience:** The User and AI Coding Assistants.
- **Tone:** Technical, concise, and brutally honest regarding  design decisions,security risks and performance bottlenecks.
- **No Fluff:** Omit user stories, time estimates, and marketing jargon.

## Analysis Steps

1. **Environment Discovery:** Run `ls -R` or equivalent to map the current directory structure.
1. **Structural Mapping:** Map the {{description}} against the discovered project structure, identifying any missing components or gaps in functionality that need filling up.
1. **Gap Analysis:** Check current project structure and identify what core implementation is missing to support these requirements.
1. **Risk Assessment:** Perform a "Pre-Mortem" analysis to identify exactly where this project is likely to fail technically or scope-creep.
1. **Generate PRD:** Create or overwrite a markdown file (`PRD.md`) with these considerations and following the specified structure to outline your product vision and strategy for this feature request until you've covered all constraints mentioned above in order of importance/urgency.  

## Example PRD structure

---

### Document Overview

[A short overview of the solution to be built. Explain briefly what problem it solves and how. Finish with a brief explanation of the criteria for success.]  

### Functional Requirements

#### Feature 1: {feature_name}

[Feature Category] (Priority: [High/Medium/Low])
[Specific feature or behavior]
[Supporting sub-features or conditions]

#### Feature N: {feature_name}

(Repeat as necessary)

### Technical Considerations

#### Technical Needs

    [Stack, platforms, frameworks, libraries]

#### Integration Points

    [3rd-party APIs, standards support, external services]

#### Data Storage

    [User data handling]

#### Privacy & Constraints

    [compliance, privacy principles, other technical or requirements constraints]
    
#### Scalability & Performance

    [Optimization strategies, performance goals]

#### Potential Challenges

    [Risks and mitigation plans]

---
