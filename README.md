# Code Assistant Resources

This repository is a collection of prompts, agent definitions, and command templates designed to structure and enhance the capabilities of a Large Language Model (LLM) based code assistant.

The organization of this project is inspired by the common phases of software development:

```mermaid
1. Discover --> 2. Design --> 3. Build --> 4. Deploy --> 5. Support & Scale
```

## Directory Structure

This project separates resources into their relevant stage:

```
/
├── global/
├── 1-discover/
│   ├── agents/
│   └── commands/
├── 2-design/
│   ├── agents/
│   └── commands/
├── 3-build/
│   ├── agents/
│   └── commands/
├── 4-deploy/
│   ├── agents/
│   └── commands/
└── 5-support-and-scale/
    ├── agents/
    └── commands/
```

-   **`/N-phase/`**: Each top-level directory corresponds to a phase in the development lifecycle.
-   **`agents/`**: Contains prompts that define specialized "agents" for complex tasks within that phase (e.g., a *debugger* agent).
-   **`commands/`**: Contains prompts for more specific, single-purpose commands (e.g., a *create-commit* command).
