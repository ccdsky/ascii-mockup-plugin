---
name: ascii-mockup
description: >
  Create ASCII wireframes, system diagrams, database schemas, and slide deck layouts for visual
  planning and iteration — before any code, assets, or databases are built.
  Use when: ASCII wireframe of, mockup a, visualize the layout of, before writing code show me,
  create a diagram of, wireframe a, or when the user describes a product idea and needs to align
  on structure before building.
---

# ASCII Mockup

## Overview

To create ASCII wireframes, system diagrams, database schemas, and slide deck layouts that let the user refine structure and layout through conversation — before any code, slides, or databases are created. Never produce code. Never suggest building. The entire purpose is visual planning and iteration.

## Domain Classification

Identify which domain the request falls into before producing the mockup:

1. **UI Wireframe** — Web apps, dashboards, landing pages, mobile screens, admin panels
2. **System / Architecture Diagram** — How components interact, tool call flows, infrastructure, APIs, workflows
3. **Data Schema** — Database tables, relationships, fields, PKs/FKs
4. **Slide Deck Layout** — Slide-by-slide structure with content placement

When a request is ambiguous, ask one clarifying question before proceeding.

## Workflow

To execute the ASCII mockup workflow, follow these four steps in order:

### Step 1: Confirm Scope

If the user's request is specific enough to proceed, start immediately. If key layout decisions are missing (e.g., "wireframe a dashboard" with no details on sections), ask one brief clarifying question — not multiple.

### Step 2: Produce the ASCII Mockup

Load `references/ascii-patterns.md` to use the correct symbols and conventions for the domain.

Rules for all mockups:
- **Maximum line width is 80 characters** — no line in the output may exceed 80
  characters. Stack sections vertically rather than side-by-side if needed to
  stay within this limit.
- Use box-drawing characters (`┌ ─ ┐ │ └ ┘ ├ ┤ ┬ ┴ ┼`) for borders and structure
- Label every region, section, or component clearly
- Show proportions and relative sizing — wider/taller elements should visually
  appear so
- Use placeholder content (`[Chart: Revenue Over Time]`, `[Hero Image]`,
  `id INT PK`) — never leave regions blank
- For UI: annotate key color intent with inline comments like `← green` or
  `← sidebar bg`
- For slides: number each slide and show a rough content block layout inside a
  labeled box
- For schemas: show table name as header, columns as rows, PK/FK annotated, and
  relationship arrows between tables
- For system diagrams: show components as boxes with labeled arrows indicating
  data/control flow

Output the mockup in a single fenced code block using plain text (no syntax
highlighting).

### Step 3: Pause and Ask for Changes

After every mockup (initial or revised), end with exactly this pattern:

```
---
What would you like to change? I can adjust layout, proportions, labels, sections, relationships, or structure.
```

Do NOT ask if they want to build it. Do NOT suggest next steps beyond refinement. Wait for their response.

### Step 4: Iterate

Apply each change they request and redraw the full mockup — never patch inline. Partial updates create confusion. After each revision, return to Step 3.

To avoid token waste on large mockups (especially slides), confirm major structural changes before redrawing: "You want to swap slides 4 and 7 and add a comparison table to slide 6 — redrawing now."

## Domain-Specific Notes

### UI Wireframes

- Render the full page/screen from top to bottom
- Sidebar widths should be visually narrower than main content
- Stat cards should appear side-by-side in a row
- Charts should be labeled with type and data axis labels
- Navigation bars go at the top; footers at the bottom

### System / Architecture Diagrams

- Use arrows (`──▶`, `◀──`, `──▶`) to show direction of data or control flow
- Group related components inside a shared outer box when they belong to the same service or layer
- Label every arrow with what it carries (`HTTP GET /users`, `SQL query`, `event: user.created`)
- Keep the layout top-to-bottom or left-to-right — avoid crossing arrows

### Data Schemas

- Show each table as a bordered box with the table name as the header
- Each row = one column: `column_name  TYPE  PK/FK/nullable`
- Use relationship lines with crow's foot notation (`──<` many, `──|` one) between tables
- Group related tables visually (e.g., auth tables clustered together)
- Add a brief plain-English relationship summary below the diagram (e.g., "Users have many Purchases via user_id")

### Slide Deck Layouts

- Show one slide per labeled box, numbered sequentially
- Inside each slide box, show the rough placement of: title, body text blocks, images, charts, bullet lists, quotes
- Note layout variation — not every slide should look the same
- Keep slides compact; this is structure, not content

## Resources

- `references/ascii-patterns.md` — Symbol library, box-drawing characters, and reusable component patterns for all four domains
