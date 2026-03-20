# NICE Claude Code Marketplace

Collection of tools for Agentic LOB use in Claude Code.

## Plugins

### Public Plugins

- **cognigy**: Cognigy AI agent development skills
  - Skills: xapp, code-node, aiagent-tool, aiagent-persona, api
  - Install: `/plugin install cognigy@nice`

- **cxone**: CXone studio integration skills
  - Install: `/plugin install cxone@nice`

- **knowledge**: Knowledge base management skills
  - Skills: get-public-content, extract-articles, scaffold-hierarchy, publish-article
  - Install: `/plugin install knowledge@nice`

### Private Plugins

- **private**: NICE APAC internal skills (private repo)
  - Requires authentication to access
  - Install: `/plugin install private@nice`

## Setup

Add this marketplace to Claude Code:

```bash
/plugin marketplace add ~/repos/claude-marketplace/nice
```

Install a plugin:

```bash
/plugin install cognigy@nice
```

## Repository Structure

```
nice/
├── .claude-plugin/
│   └── marketplace.json          # Marketplace catalog
├── plugins/
│   ├── cognigy/                  # Submodule: public
│   ├── cxone/                    # Submodule: public
│   ├── knowledge/                # Submodule: public
│   └── private/                  # Submodule: private
└── README.md
```

Each plugin is a separate repository maintained as a git submodule.
