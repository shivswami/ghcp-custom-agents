# Awesome Custom Agents

Prompts that help you discover and generate curated GitHub Copilot Custom Agents 

**Tags:** github-copilot, agents, discovery, meta, prompt-engineering, agents, architecture, code-analysis, diagram-generation, devexp

## Items in this Collection

| Title | Type | Description | Tools access |
| ----- | ---- | ----------- | ----------- |
| [Architecture Explainer](.github/agents/1-Arch.md) | Agent | Analyze large enterprise repositories and monorepos to produce a comprehensive, high-level architecture explanation. Specializes in reverse-engineering and documenting complex enterprise codebases, identifying system boundaries, components, and integration points. | edit, search, new, runCommands, vscodeAPI, problems, changes, fetch, githubRepo |
| [Component Mapper](.github/agents/2-Map.md) | Agent | Map architecture components from GitDiagram context to concrete code locations, enabling interactive diagram navigation and code exploration. Creates explicit mappings between architectural components and actual code locations for large enterprise repositories. | edit, search, new, runCommands, vscodeAPI, problems, changes, fetch, githubRepo |
| [ Mermaid Diagram Generator](.github/agents/3-Visualise.md) | Agent | Generate interactive, vertical Mermaid.js system architecture diagrams from architecture context and component mappings. Specializes in creating clear, interactive, and accurate system architecture diagrams using Mermaid.js with clickable nodes. | edit, search, new, runCommands, vscodeAPI, problems, changes, fetch, githubRepo |

## Pipeline Workflow

The GitDiagram agents are designed to work in sequence for comprehensive repository analysis:

1. **Architecture Explainer** (Agent 1) → Analyzes repository structure and generates architecture context
2. **Component Mapper** (Agent 2) → Maps architectural components to code locations
3. **Mermaid Diagram Generator** (Agent 3) → Creates interactive visual diagrams

## Usage Instructions

### For Architecture Analysis
1. Run **Agent 1** to analyze your repository and generate `context.md`
2. Run **Agent 2** to map components to code locations
3. Run **Agent 3** to generate interactive Mermaid diagrams

### For Code Reviews
- Use the **Code Review Skill** when performing code reviews or evaluating pull requests
- Follow the comprehensive checklist for security, performance, and quality assessment

## Features

- **Enterprise Repository Support**: Optimized for large monorepos and complex architectures
- **Evidence-Based Analysis**: Distinguishes between confirmed facts, inferred patterns, and assumptions
- **Interactive Diagrams**: Generates Mermaid.js diagrams with clickable navigation to code
- **Confidence Levels**: Clearly marks analysis confidence (HIGH, MEDIUM, LOW, UNCERTAIN)
- **Comprehensive Code Review**: Covers security, performance, testing, and maintainability aspects

## Repository Structure

```
.github/
├── agents/
│   ├── 1-Arch.md          # Architecture Explainer Agent
│   ├── 2-Map.md           # Component Mapper Agent
│   └── 3-Visualise.md     # Mermaid Diagram Generator Agent
└── skills/
    └──                    # TBC Skill
```

## Contributing

To add new agents or skills to this collection:

1. Create agent files in `.github/agents/` directory
2. Create skill files in `.github/skills/` directory
3. Update this table with the new entry following the established format
4. Follow the naming conventions and structure patterns

## License

This collection is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.