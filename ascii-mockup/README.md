# ASCII Mockup Plugin

A Claude Desktop CoWork plugin for creating ASCII wireframes, system diagrams, data schemas, and slide deck layouts — for visual planning and iteration before any code or assets are built.

## What It Does

Describe what you want to visualize and Claude will produce a detailed ASCII mockup. Iterate through conversation until the structure is right — then go build it.

**Supported domains:**
- UI Wireframes — dashboards, landing pages, mobile screens, admin panels
- System / Architecture Diagrams — component interactions, API flows, infrastructure
- Data Schemas — tables, relationships, PKs/FKs with crow's foot notation
- Slide Deck Layouts — slide-by-slide structure with content placement

## Trigger Phrases

- "ASCII wireframe of..."
- "Mockup a..."
- "Visualize the layout of..."
- "Before writing code, show me..."
- "Create a diagram of..."
- "Wireframe a..."

## Plugin Structure

```
ascii-mockup-builder/
├── .claude-plugin/
│   └── plugin.json               # Plugin manifest
├── skills/
│   └── ascii-mockup/
│       ├── SKILL.md              # Skill instructions and workflow
│       └── references/
│           └── ascii-patterns.md # Symbol library and component patterns
└── README.md
```

## Installation

1. Clone or download this directory
2. Open **Claude Desktop** → Settings → Plugins
3. Click **Add local plugin** and select this directory
4. The `ascii-mockup` skill is now available in any conversation

## Usage

Simply describe what you want to wireframe. Claude will:
1. Identify the domain (UI, diagram, schema, or slides)
2. Ask one clarifying question if needed
3. Produce the full ASCII mockup in a code block
4. Prompt you for changes and iterate until it's right

## Example Prompts

```
Wireframe a SaaS dashboard with a sidebar, stat cards, a revenue chart, and a data table.

Create a system architecture diagram for a REST API with auth, caching, and a database layer.

ASCII mockup of a 3-table database schema for users, orders, and products.

Slide deck layout for a 10-slide investor pitch deck.
```
