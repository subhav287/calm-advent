# My Advent of CALM Journey

This repository tracks my 24-day journey learning the Common Architecture Language Model (CALM).

## Progress

- [x] Day 1: Install CALM CLI and Initialize Repository
- [x] Day 2: Create Your First Node
- [x] Day 3: Connect Nodes with Relationships
...

## Tools

### CALM CLI

The command-line interface for working with CALM architectures.

**Installed:** Day 1

**What it's used for:**
- **Generation**: Create architecture scaffolds from patterns using `calm generate`
- **Validation**: Validate architectures and patterns against the CALM 1.1 schema using `calm validate`
- **Templates**: Generate documentation and configuration files from architectures using `calm template` or `calm docify`

**Basic commands:**
```bash
# Validate an architecture file
calm validate -a architectures/my-first-architecture.json

# Validate a pattern
calm validate -p patterns/my-pattern.json

# Full validation (architecture against pattern)
calm validate -p patterns/my-pattern.json -a architectures/my-first-architecture.json

# Generate an architecture from a pattern
calm generate -p patterns/my-pattern.json -o architectures/generated.json

# Generate documentation
calm docify -a architectures/my-first-architecture.json -o ./docs
```

### CALM VSCode Extension

Visual editor and previewer for CALM architectures within VS Code.

**Installed:** Day 4

**Marketplace:** [FINOS.calm-vscode-plugin](https://marketplace.visualstudio.com/items?itemName=FINOS.calm-vscode-plugin)

**What it provides:**
- **Visualization**: Interactive diagrams showing nodes, relationships, and system composition
- **Tree Navigation**: Hierarchical view of architecture elements (nodes, relationships, flows, controls)
- **Live Preview**: Real-time architecture preview as you edit JSON files
- **Syntax Highlighting**: CALM-aware editing with schema validation hints
- **Quick Navigation**: Jump between referenced nodes and relationships

**Keyboard Shortcut:**
- Open CALM preview panel: `Ctrl+Shift+C` (Windows/Linux) or `Cmd+Shift+C` (macOS)

### How Tools Work Together

The CALM CLI and VSCode Extension complement each other in a complete workflow:

1. **Edit in VSCode**: Use the extension to visualize your architecture in real-time while editing JSON
2. **Live Preview**: See changes instantly in the preview panel — no manual refresh needed
3. **Validate with CLI**: Run `calm validate` from the terminal to catch schema errors and linting warnings before committing
4. **Generate Docs**: Use `calm docify` to produce documentation websites from validated architectures
5. **Iterate**: Fix validation errors, preview changes, and refine until ready to deploy

This tight integration keeps your workflow fast and reduces round-trip time between editing, validation, and visualization.

## Architectures

This directory will contain CALM architecture files documenting systems.

## Patterns

This directory will contain CALM patterns for architectural governance.

## Docs

Generated documentation from CALM models.