# ASCII Mockup Pattern Library

## Box-Drawing Characters

```
Single border:  ┌ ─ ┐ │ └ ┘ ├ ┤ ┬ ┴ ┼
Double border:  ╔ ═ ╗ ║ ╚ ╝ ╠ ╣ ╦ ╩ ╬
Mixed:          ╒ ╕ ╘ ╛ ╞ ╡ ╤ ╧ ╪  (single horizontal, double vertical)
Arrows:         ──▶  ◀──  ──▷  ▶──  ↑  ↓  ←  →  ↔  ↕
Crow's foot:    ──<  >──  ──|  |──  ──o  o──
Separators:     ━━━  ═══  ···  ---  ___
Bullets:        •  ○  ▸  ▪  ◦
Status:         ✓  ✗  ●  ○  ◐  □  ■
```

---

## UI Wireframe Patterns

### Dashboard Layout (sidebar + main)
```
┌──────────────────────────────────────────────────────┐
│  ┌──────────┐  ┌──────────────────────────────────┐  │
│  │  SIDEBAR │  │           TOP NAV / HEADER        │  │
│  │          │  ├──────────────────────────────────┤  │
│  │ ▸ Nav 1  │  │  ┌────────┐ ┌────────┐ ┌──────┐  │  │
│  │ ▸ Nav 2  │  │  │ STAT 1 │ │ STAT 2 │ │STAT 3│  │  │
│  │ ▸ Nav 3  │  │  └────────┘ └────────┘ └──────┘  │  │
│  │          │  ├──────────────────┬─────────────┤  │  │
│  │          │  │ [Chart: Line]    │ [Chart: Pie] │  │  │
│  │          │  │                  │              │  │  │
│  │          │  ├──────────────────┴─────────────┤  │  │
│  │          │  │          DATA TABLE             │  │  │
│  │          │  │  Col A    Col B    Col C    Col D│  │  │
│  │          │  │  ──────  ──────  ──────  ──────  │  │
│  │          │  │  row 1    ...      ...      ...  │  │
│  └──────────┘  └──────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```

### Stat Card Row
```
┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐
│  Total Users     │  │  Revenue         │  │  Conversion      │  │  MRR             │
│  ─────────────── │  │  ─────────────── │  │  ─────────────── │  │  ─────────────── │
│  12,483          │  │  $48,200         │  │  3.4%            │  │  $9,600          │
│  ↑ 12% vs last  │  │  ↑ 8% vs last   │  │  ↓ 0.2%         │  │  ↑ 5% vs last   │
└──────────────────┘  └──────────────────┘  └──────────────────┘  └──────────────────┘
```

### Navigation Bar
```
┌────────────────────────────────────────────────────────────────────────────────┐
│  [Logo]     Home    Features    Pricing    Docs    Blog          Sign In  Get Started │
└────────────────────────────────────────────────────────────────────────────────┘
```

### Hero Section
```
┌──────────────────────────────────────────────────────────────┐
│                                                              │
│              The fastest way to ship your                    │
│                    next big idea.                            │
│                                                              │
│         Stop wasting time. Start building faster.           │
│                                                              │
│         [ Get Started Free ]    [ Watch Demo → ]            │
│                                                              │
│  ┌────────────────────────────────────────────────────┐     │
│  │                [Product Screenshot]                │     │
│  └────────────────────────────────────────────────────┘     │
│                                                              │
└──────────────────────────────────────────────────────────────┘
```

### Social Proof / Logo Bar
```
┌──────────────────────────────────────────────────────────────┐
│          Trusted by teams at                                 │
│   [Logo]    [Logo]    [Logo]    [Logo]    [Logo]             │
└──────────────────────────────────────────────────────────────┘
```

### Features Grid (3-column)
```
┌────────────────────────────────────────────────────────────────┐
│  ┌──────────────┐    ┌──────────────┐    ┌──────────────┐     │
│  │  [Icon]      │    │  [Icon]      │    │  [Icon]      │     │
│  │  Feature 1   │    │  Feature 2   │    │  Feature 3   │     │
│  │  ──────────  │    │  ──────────  │    │  ──────────  │     │
│  │  Short desc  │    │  Short desc  │    │  Short desc  │     │
│  └──────────────┘    └──────────────┘    └──────────────┘     │
└────────────────────────────────────────────────────────────────┘
```

### Pricing Cards (3 tiers)
```
┌──────────────┐   ┌══════════════╗   ┌──────────────┐
│  Free        │   ║  Pro  ★      ║   │  Enterprise  │
│  $0/mo       │   ║  $29/mo      ║   │  Custom      │
│  ──────────  │   ╠══════════════╣   │  ──────────  │
│  • Feature A │   ║  • Feature A ║   │  • All Pro   │
│  • Feature B │   ║  • Feature B ║   │  • Priority  │
│  • Feature C │   ║  • Feature C ║   │  • SLA       │
│              │   ║  • Feature D ║   │  • SSO       │
│  [Get Free]  │   ║  [Start Pro] ║   │  [Contact]   │
└──────────────┘   ╚══════════════╝   └──────────────┘
```
*(double border = highlighted/recommended tier)*

### Data Table
```
┌────────────────────────────────────────────────────────┐
│  NAME              STATUS     PLAN       JOINED        │
│  ──────────────    ──────     ──────     ──────────    │
│  Alice Martin      ● Active   Pro        Jan 12, 2025  │
│  Bob Chen          ● Active   Free       Feb 3, 2025   │
│  Carol White       ○ Inactive Pro        Dec 1, 2024   │
│  David Kim         ● Active   Enterprise Mar 5, 2025   │
└────────────────────────────────────────────────────────┘
```
*(● = active/green implied, ○ = inactive/gray implied)*

### Footer
```
┌────────────────────────────────────────────────────────────────┐
│  [Logo]   © 2025 Company Inc                                   │
│                                                                │
│  Product        Company        Resources      Legal           │
│  Features       About          Blog           Privacy         │
│  Pricing        Careers        Docs           Terms           │
│  Changelog      Contact        Status                         │
└────────────────────────────────────────────────────────────────┘
```

### Mobile Screen
```
┌────────────┐
│ ☰   Title  │  ← top nav
├────────────┤
│ [Hero Img] │
│            │
│  Heading   │
│  Sub text  │
│ [  CTA   ] │
├────────────┤
│  Section   │
│  ──────    │
│  Content   │
│            │
├────────────┤
│ 🏠  📊  👤 │  ← bottom tab bar
└────────────┘
```

---

## System / Architecture Diagram Patterns

### Layered System
```
┌─────────────────────────────────────────────────────────┐
│                        CLIENT                           │
│   Browser / Mobile App / CLI                            │
└───────────────────────┬─────────────────────────────────┘
                        │  HTTPS
                        ▼
┌─────────────────────────────────────────────────────────┐
│                      API GATEWAY                        │
│   Auth  │  Rate Limit  │  Routing                       │
└────────────┬──────────────────────┬──────────────────────┘
             │                      │
             ▼                      ▼
┌────────────────────┐   ┌──────────────────────┐
│   Service A        │   │   Service B           │
│   (Users / Auth)   │   │   (Billing / Plans)   │
└──────────┬─────────┘   └──────────┬────────────┘
           │                        │
           ▼                        ▼
┌─────────────────────────────────────────────────┐
│                   DATABASE LAYER                │
│   ┌──────────────┐        ┌──────────────┐     │
│   │  Postgres    │        │  Redis Cache │     │
│   │  (primary)   │        │              │     │
│   └──────────────┘        └──────────────┘     │
└─────────────────────────────────────────────────┘
```

### Tool Call / Agent Flow
```
  User Prompt
      │
      ▼
┌─────────────────┐
│   Claude Agent  │
│  (orchestrator) │
└───────┬─────────┘
        │ decides tool
        ▼
┌───────────────────────────────────────────────────┐
│                   TOOL DISPATCH                   │
│                                                   │
│  ┌──────────┐  ┌──────────┐  ┌────────────────┐  │
│  │  Bash    │  │  Glob /  │  │  WebFetch /    │  │
│  │  (exec)  │  │  Grep    │  │  WebSearch     │  │
│  └────┬─────┘  └────┬─────┘  └───────┬────────┘  │
│       │             │                │            │
└───────┼─────────────┼────────────────┼────────────┘
        │             │                │
        ▼             ▼                ▼
     stdout        file paths       HTML/JSON
        │             │                │
        └─────────────┴────────────────┘
                       │
                       ▼
               tool_result back
               to Claude context
```

### Request/Response Flow
```
Client ──▶ [Load Balancer] ──▶ [App Server] ──▶ [Cache] ──▶ HIT ──▶ Client
                                     │                    MISS
                                     ▼                      │
                              [Database] ◀───────────────────┘
                                     │
                              result ──▶ Cache ──▶ Client
```

---

## Data Schema Patterns

### Table Block
```
┌──────────────────────────────┐
│  USERS                       │
├──────────────────────────────┤
│  id          UUID     PK     │
│  email       TEXT     UNIQUE │
│  name        TEXT            │
│  created_at  TIMESTAMP       │
│  plan_id     UUID     FK ──▶ │
└──────────────────────────────┘
```

### Multi-Table Schema with Relationships
```
┌─────────────────────┐         ┌──────────────────────┐
│  USERS              │         │  PRODUCTS             │
├─────────────────────┤         ├──────────────────────┤
│  id         UUID PK │──┐   ┌──│  id         UUID PK  │
│  email      TEXT    │  │   │  │  name       TEXT     │
│  name       TEXT    │  │   │  │  price      DECIMAL  │
│  created_at TSTZ    │  │   │  │  created_at TSTZ     │
└─────────────────────┘  │   │  └──────────────────────┘
                         │   │
                         ▼   ▼
              ┌───────────────────────────┐
              │  PURCHASES                │
              ├───────────────────────────┤
              │  id          UUID  PK     │
              │  user_id     UUID  FK──▶ USERS   │
              │  product_id  UUID  FK──▶ PRODUCTS│
              │  amount      DECIMAL      │
              │  created_at  TSTZ         │
              └───────────────────────────┘
                         │
                         ▼
              ┌───────────────────────────┐
              │  AUDIT_LOGS               │
              ├───────────────────────────┤
              │  id          UUID  PK     │
              │  user_id     UUID  FK     │
              │  action      TEXT         │
              │  metadata    JSONB        │
              │  created_at  TSTZ         │
              └───────────────────────────┘

Relationships:
  Users ──< Purchases  (one user → many purchases)
  Products ──< Purchases  (one product → many purchases)
  Users ──< Audit_Logs  (one user → many log entries)
```

---

## Slide Deck Patterns

### Title Slide
```
┌──────────────────────────────────────────────────────┐
│  SLIDE 1 — Title                                     │
│  ┌────────────────────────────────────────────────┐  │
│  │                                                │  │
│  │         [Company Logo]                         │  │
│  │                                                │  │
│  │   REPLACING MANUAL REPORTING                   │  │
│  │   WITH AUTOMATED DASHBOARDS                    │  │
│  │                                                │  │
│  │   Subtitle: How to reclaim 10 hrs/week         │  │
│  │                                                │  │
│  │   Presenter Name  |  Date  |  Audience         │  │
│  │                                                │  │
│  └────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```

### Problem Slide
```
┌──────────────────────────────────────────────────────┐
│  SLIDE 2 — The Problem                               │
│  ┌────────────────────────────────────────────────┐  │
│  │  The Problem With Manual Reporting             │  │
│  │  ─────────────────────────────────            │  │
│  │                                                │  │
│  │  • Point one about the pain                   │  │
│  │  • Point two about the cost                   │  │
│  │  • Point three about the risk                 │  │
│  │                                                │  │
│  │  ┌──────────────────┐                          │  │
│  │  │ [Supporting stat │                          │  │
│  │  │  or image here]  │                          │  │
│  │  └──────────────────┘                          │  │
│  └────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```

### Two-Column Slide
```
┌──────────────────────────────────────────────────────┐
│  SLIDE 4 — Before vs After                           │
│  ┌────────────────────────────────────────────────┐  │
│  │  Section Title                                 │  │
│  │  ┌───────────────────┐ ┌───────────────────┐   │  │
│  │  │  BEFORE           │ │  AFTER            │   │  │
│  │  │  ───────────────  │ │  ───────────────  │   │  │
│  │  │  • Manual step 1  │ │  • Automated ✓   │   │  │
│  │  │  • Manual step 2  │ │  • Automated ✓   │   │  │
│  │  │  • Manual step 3  │ │  • Automated ✓   │   │  │
│  │  │  [Red/bad]        │ │  [Green/good]     │   │  │
│  │  └───────────────────┘ └───────────────────┘   │  │
│  └────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```

### Big Quote Slide
```
┌──────────────────────────────────────────────────────┐
│  SLIDE 7 — Key Insight                               │
│  ┌────────────────────────────────────────────────┐  │
│  │                                                │  │
│  │                                                │  │
│  │   "  The teams that move fastest are the       │  │
│  │      ones who stopped asking for reports       │  │
│  │      and started reading dashboards.  "        │  │
│  │                                                │  │
│  │              — Source / Attribution            │  │
│  │                                                │  │
│  └────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```

### 3-Up Card Row Slide
```
┌──────────────────────────────────────────────────────┐
│  SLIDE 5 — Three Key Benefits                        │
│  ┌────────────────────────────────────────────────┐  │
│  │  Why This Works                                │  │
│  │  ┌────────────┐  ┌────────────┐  ┌──────────┐  │  │
│  │  │  [Icon 1]  │  │  [Icon 2]  │  │ [Icon 3] │  │  │
│  │  │  Benefit A │  │  Benefit B │  │Benefit C │  │  │
│  │  │  ────────  │  │  ────────  │  │ ───────  │  │  │
│  │  │  Desc      │  │  Desc      │  │ Desc     │  │  │
│  │  └────────────┘  └────────────┘  └──────────┘  │  │
│  └────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```

### CTA / Close Slide
```
┌──────────────────────────────────────────────────────┐
│  SLIDE 10 — Close / CTA                              │
│  ┌────────────────────────────────────────────────┐  │
│  │                                                │  │
│  │         Ready to get started?                  │  │
│  │                                                │  │
│  │         [  Book a Demo  ]                      │  │
│  │                                                │  │
│  │   contact@company.com  |  company.com/demo     │  │
│  │                                                │  │
│  │   [QR Code placeholder]                        │  │
│  │                                                │  │
│  └────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────┘
```
