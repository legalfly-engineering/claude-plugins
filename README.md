# LegalFly Plugins

Plugins that turn Claude into a legal specialist powered by LegalFly Discovery AI. Built for [Claude Cowork](https://claude.com/product/cowork), also compatible with [Claude Code](https://claude.com/product/claude-code).

## Available Plugins

| Plugin                     | How it helps                                                                                                                               | Connectors   |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------ |
| **[legalfly](./legalfly)** | Query legal documents, discover relevant clauses, analyze contracts, and research across your document corpus using LegalFly Discovery AI. | LegalFly API |

## Installation

Install the plugin directly from GitHub:

```bash
claude plugin install github:legalfly/claude-plugins/legalfly
```

Once installed, the plugin activates automatically. The `discover` tool becomes available for querying your legal documents.

## How Plugins Work

The plugin follows this structure:

```text
legalfly/
├── .claude-plugin/plugin.json   # Manifest
└── mcp.json                     # Tool connections
```

The plugin connects Claude to LegalFly's Discovery AI via [MCP servers](https://modelcontextprotocol.io/). Everything is file-based — just JSON, no code, no infrastructure, no build steps.

## The Discover Tool

The `discover` tool connects Claude to LegalFly's Discovery AI, enabling:

- **Document queries** — Ask natural language questions across your legal document corpus
- **Clause discovery** — Find specific clauses, terms, and provisions across contracts
- **Legal research** — Search for relevant precedents, definitions, and legal concepts
- **Multi-document analysis** — Compare and analyze multiple documents simultaneously
