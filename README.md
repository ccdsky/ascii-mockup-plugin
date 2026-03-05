# ASCII Mockup Plugin

Create ASCII wireframes, dashboards, system diagrams, data schemas, and slide
deck layouts for visual planning and iteration — before building anything.

Works in both **Claude Desktop (CoWork)** and **Claude Code**.

## Install in Claude Desktop (CoWork)

1. Open Claude Desktop → Settings → Plugins
2. Click **Add marketplace from GitHub**
3. Enter: `https://github.com/ccdsky/ascii-mockup-plugin`
4. Install the `ascii-mockup` plugin

## Install in Claude Code

```bash
cp -r ascii-mockup/skills/ascii-mockup ~/.claude/skills/ascii-mockup
```

Or clone and copy:

```bash
git clone https://github.com/ccdsky/ascii-mockup-plugin
cp -r ascii-mockup-plugin/ascii-mockup/skills/ascii-mockup ~/.claude/skills/
```

## Plugins

| Plugin | Description |
|--------|-------------|
| [ascii-mockup](./ascii-mockup) | ASCII wireframes, dashboards, diagrams, schemas, and slide layouts |

## Usage

Just describe what you want to visualize — the skill activates automatically:

- "ASCII wireframe of a SaaS dashboard"
- "Mockup a mobile onboarding flow"
- "Diagram the architecture for a REST API"
- "Wireframe a 10-slide pitch deck"
- "Create a database schema for an e-commerce app"

## Author

Chris Cappelli
