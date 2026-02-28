# Top Design Systems — Claude Code Skill

A [Claude Code](https://claude.ai/claude-code) skill that gives Claude deep knowledge of the **top 20 design systems** used by the world's leading tech companies, sourced from [UI Guideline's](https://www.uiguideline.com) annual survey.

When installed, Claude uses this knowledge during your **planning phase** to make better-informed decisions about component architecture, design tokens, accessibility, theming, and technology choices — grounded in real patterns from production design systems at Google, Microsoft, Adobe, Shopify, GitHub, IBM, and more.

## What This Skill Does

During project planning, Claude will:

- **Match your tech stack** to the most relevant design systems (React, Vue, Angular, Web Components, multi-platform)
- **Match your use case** to proven patterns (e-commerce, enterprise, developer tools, creative tools, etc.)
- **Recommend architecture** for design tokens, theming, accessibility, and component APIs based on what works at scale
- **Reference 60+ component patterns** analyzed across all 20 systems (buttons, modals, tables, forms, navigation, and more)
- **Link directly to source repos** so you can study implementations

## The 20 Design Systems

| # | Design System | Company | GitHub |
|---|---|---|---|
| 1 | Material Design | Google | [material-components](https://github.com/material-components) |
| 2 | Atlassian Design | Atlassian | [Bitbucket](https://bitbucket.org/atlassian/atlassian-frontend-mirror) |
| 3 | Polaris | Shopify | [Shopify/polaris](https://github.com/Shopify/polaris) |
| 4 | Ant Design | XTech | [ant-design](https://github.com/ant-design/ant-design) |
| 5 | Fluent 2 | Microsoft | [microsoft/fluentui](https://github.com/microsoft/fluentui) |
| 6 | Primer | GitHub | [primer](https://github.com/primer) |
| 7 | Garden | Zendesk | [zendeskgarden](https://github.com/zendeskgarden) |
| 8 | Spectrum | Adobe | [adobe/react-spectrum](https://github.com/adobe/react-spectrum) |
| 9 | Chakra UI | Community | [chakra-ui](https://github.com/chakra-ui/chakra-ui) |
| 10 | Carbon | IBM | [carbon-design-system](https://github.com/carbon-design-system) |
| 11 | Base Web | Uber | [uber/baseweb](https://github.com/uber/baseweb) |
| 12 | Elastic UI | Elastic | [elastic/eui](https://github.com/elastic/eui) |
| 13 | Pajamas | GitLab | [GitLab](https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com) |
| 14 | Vuetify | Community | [vuetifyjs/vuetify](https://github.com/vuetifyjs/vuetify) |
| 15 | Mantine | Community | [mantinedev/mantine](https://github.com/mantinedev/mantine) |
| 16 | Material UI (MUI) | Community | [mui](https://github.com/mui) |
| 17 | Radix | WorkOS | [radix-ui](https://github.com/radix-ui) |
| 18 | Blueprint | Palantir | [palantir/blueprint](https://github.com/palantir/blueprint) |
| 19 | Angular Material | Google | [angular/components](https://github.com/angular/components) |
| 20 | Pluralsight Design | Pluralsight | [pluralsight/classic-design-system](https://github.com/pluralsight/classic-design-system) |

## Installation

### Option 1 — Clone Into Your Project (Recommended)

Copy the skill file directly into your project's Claude Code skills directory:

```bash
# From your project root
mkdir -p .claude/skills

# Download the skill file
curl -o .claude/skills/top-design-systems.md \
  https://raw.githubusercontent.com/oldbrush/skill-top-design-systems/main/.claude/skills/top-design-systems.md
```

### Option 2 — Clone the Entire Repo

```bash
git clone https://github.com/oldbrush/skill-top-design-systems.git
cp skill-top-design-systems/.claude/skills/top-design-systems.md /path/to/your/project/.claude/skills/
```

### Option 3 — Manual Copy

1. Go to [`.claude/skills/top-design-systems.md`](.claude/skills/top-design-systems.md) in this repo
2. Copy the raw contents
3. Create `.claude/skills/top-design-systems.md` in your project
4. Paste the contents and save

### Verify Installation

After installing, start Claude Code in your project and ask:

```
What design system would you recommend for a React e-commerce dashboard?
```

Claude should reference specific systems like Polaris (Shopify), Ant Design, and MUI with details about their component counts, token systems, and accessibility approaches.

## How It Works

Claude Code loads skill files from `.claude/skills/` in your project directory. When a skill file is present, Claude has access to that knowledge during your entire conversation.

This skill activates when you're:
- Planning a new frontend project or component library
- Choosing a design system or UI framework
- Making decisions about theming, tokens, or accessibility architecture
- Designing component APIs or composition patterns
- Evaluating technology choices for UI development

## What's Inside the Skill

The skill file contains:

1. **All 20 design systems** with framework, component count, design tokens strategy, WCAG compliance level, theming approach, best-use-case, and key architectural patterns
2. **60+ component taxonomy** organized into 10 categories (Data Display, Inputs, Overlays, Buttons, Controls, Navigation, Notifications, Loaders, States, Atomic Elements)
3. **Planning Decision Framework** with three steps:
   - Technology Match — maps your framework to the best systems
   - Use Case Match — maps your project type to proven patterns
   - Architecture Decisions — recommendations for tokens, accessibility, theming, and component APIs
4. **Quick Reference Links** to every GitHub repo and documentation site

## Example Conversations

**Planning a new project:**
> "I'm building a data analytics dashboard in React. What design patterns should I follow?"

Claude will reference Elastic UI (data-dense interfaces), Blueprint (Palantir's desktop-optimized system), and Carbon (IBM's enterprise patterns), with specific recommendations for component architecture and data visualization.

**Choosing a token strategy:**
> "How should I structure my design tokens?"

Claude will compare the two-layer approach (Fluent 2, Angular Material), three-layer approach (Material Design), and CSS custom properties patterns used across all 20 systems.

**Accessibility planning:**
> "What's the best approach for accessible components?"

Claude will recommend React Aria (Adobe Spectrum) for accessible hooks, Radix Primitives for unstyled accessible components, and reference Primer's 9-mode accessibility system.

## Data Source

All design system data is sourced from:
- [UI Guideline](https://www.uiguideline.com) — annual survey of hundreds of developers and designers ranking the top 20 design systems
- Official GitHub repositories and documentation sites of each design system

## Contributing

Contributions are welcome! If a design system has updated its component count, accessibility level, or architecture, please open a PR with the correction and a link to the source.

## License

MIT — see [LICENSE](LICENSE)
