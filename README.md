# GitHub Copilot Custom Agents

A collection of custom GitHub Copilot agents and skills that developers can use to enhance their coding experience.

## What are Custom Agents?

GitHub Copilot allows you to create custom agents that follow your specific instructions and workflows. These agents can be tailored for:
- Specific programming languages and frameworks
- Code review patterns
- Testing strategies
- Documentation styles
- Development workflows

## Directory Structure

```
.github/
├── agents/     # Custom agent configurations
└── skills/     # Custom skill definitions
```

## Available Agents

<!-- Add your agents here -->

## How to Use

1. Copy the agent configuration files to your own repository's `.github/agents/` directory
2. Configure GitHub Copilot to use these agents, specifically the Tools section.
3. Start coding with your custom workflows!

## Contributing

To add your own custom agents:

1. Create a new `.md` file in the appropriate directory
2. Follow the template structure
3. Include clear instructions and examples
4. Submit a pull request

## Templates

See the `templates/` directory for agent and skill templates.

##  References
Official GitHub Copilot Docs - https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-custom-agents?search-overlay-input=GitHub+Copilot+workflow&search-overlay-ask-ai=true

Bringing Anthropic Skills to GitHub Copilot https://tiberriver256.github.io/ai%20and%20technology/skills-catalog-part-1-indexing-ai-context/

## Acknowledgements
Shoutout to Ahmad Khaleel's gitdiagram project on Github https://github.com/ahmedkhaleel2004

https://github.com/ahmedkhaleel2004/gitdiagram/tree/main

# Workflow 
cd Users/shiv/garage/proj/shiv/ghcp-custom-agents

gh repo create ghcp-custom-agents --public --source=. --remote=origin --push

git remote -v
git status
