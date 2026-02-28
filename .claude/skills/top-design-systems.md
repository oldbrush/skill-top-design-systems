# Top Design Systems Reference — Claude Code Planning Skill

> Source: [UI Guideline](https://www.uiguideline.com) — Annual survey of the top 20 design systems used by companies worldwide.

## Purpose

When planning frontend projects, use this skill to inform component architecture, design token strategy, accessibility approach, theming, and technology choices based on proven patterns from the world's most adopted design systems.

## TRIGGER

Activate this skill when the user is:
- Planning a new frontend project or UI component library
- Choosing a design system or component framework
- Making architectural decisions about theming, tokens, or accessibility
- Designing component APIs or composition patterns
- Evaluating technology choices for UI development

---

## The Top 20 Design Systems

### Tier 1 — Industry Leaders (Top 5)

#### 1. Material Design — Google
- **Site**: https://m3.material.io/
- **GitHub**: https://github.com/material-components
- **Framework**: Web Components, Android, iOS, Flutter (multi-platform)
- **Components**: ~30+ in Material Web specification
- **Design Tokens**: Yes — dynamic color system with tonal palettes, global and component-level tokens, CSS custom properties
- **Accessibility**: WCAG 2.1 AA — dynamic color meets contrast by default, minimum touch targets, responsive type
- **Theming**: Dynamic color theming ("Material You"), light/dark modes, custom brand themes via tokens
- **Best For**: Cross-platform apps, Android-first products, apps needing adaptive/expressive design
- **Key Pattern**: Three-layer token architecture (reference → system → component tokens)

#### 2. Atlassian Design System — Atlassian
- **Site**: https://atlassian.design/
- **Repo**: https://bitbucket.org/atlassian/atlassian-frontend-mirror/src/master/
- **Framework**: React
- **Design Tokens**: Yes — comprehensive token system for colors, spacing, typography
- **Accessibility**: WCAG 2.1 AA — inclusive design principles baked into every component
- **Theming**: Token-based theming with light/dark mode support
- **Best For**: Productivity tools, project management interfaces, collaboration software
- **Key Pattern**: Experience-driven design with strong content guidelines

#### 3. Polaris — Shopify
- **Site**: https://polaris.shopify.com/
- **GitHub**: https://github.com/Shopify/polaris
- **Framework**: Web Components (migrated from React for framework independence)
- **Components**: ~60+ across actions, layout, navigation, forms, tables, feedback, overlays
- **Design Tokens**: Yes — CSS custom properties (`--p-color-text`, `--p-space-500`), exported as CSS vars and JSON
- **Accessibility**: WCAG 2.1 AA — ARIA standards, keyboard navigation, screen reader support
- **Theming**: Customizable themes via design tokens, AppProvider theming
- **Best For**: E-commerce admin interfaces, merchant-facing tools, SaaS dashboards
- **Key Pattern**: Merchant productivity focus — reduce cognitive load, increase efficiency

#### 4. Ant Design — XTech
- **Site**: https://ant.design/
- **GitHub**: https://github.com/ant-design/ant-design
- **Framework**: React (primary), Vue (Ant Design Vue), Angular (NG-ZORRO)
- **Components**: ~68 across General, Navigation, Data Entry, Data Display, Feedback, Other
- **Design Tokens**: Yes — v5.0 CSS-in-JS token system with seed, map, and alias tokens
- **Accessibility**: Partial — color contrast adherence, keyboard navigation improving, weaker than peers
- **Theming**: ConfigProvider-based, dynamic theme switching, component-level style overrides
- **Best For**: Enterprise admin panels, data-heavy applications, Chinese market products
- **Key Pattern**: Four design values — Natural, Certain, Meaningful, Growing

#### 5. Fluent 2 — Microsoft
- **Site**: https://fluent2.microsoft.design/
- **GitHub**: https://github.com/microsoft/fluentui
- **Framework**: React (v9), Web Components, WinUI, iOS, Android, .NET MAUI
- **Components**: ~60+ stable in React v9
- **Design Tokens**: Yes — two-layer system (global tokens → alias/semantic tokens), 64+ layout tokens
- **Accessibility**: WCAG 2.1 AA+ — accessible by default, 4.5:1 contrast, focus management, ARIA built-in
- **Theming**: Token-based adaptive theming, light/dark mode, brand theming at any DOM level
- **Best For**: Microsoft ecosystem products, enterprise apps, cross-platform desktop/mobile
- **Key Pattern**: Five pillars — Light, Depth, Motion, Material, Scale

---

### Tier 2 — Proven & Mature (6–10)

#### 6. Primer — GitHub
- **Site**: https://primer.style/
- **GitHub**: https://github.com/primer
- **Framework**: React, CSS, ViewComponents (Rails)
- **Components**: ~80 components (one of the largest libraries)
- **Design Tokens**: Yes — CSS variables and Figma variables via `@primer/primitives`
- **Accessibility**: WCAG 2.1 AA — **nine accessibility modes** (light, dark, dimmed, high-contrast, color-vision-deficiency themes)
- **Theming**: Multiple theme variants per mode, color-blind-safe themes
- **Best For**: Developer tools, code-centric interfaces, documentation platforms
- **Key Pattern**: Accessibility-mode system with 9 distinct visual modes

#### 7. Garden — Zendesk
- **Site**: https://garden.zendesk.com/
- **GitHub**: https://github.com/zendeskgarden
- **Framework**: React (multi-package monorepo)
- **Components**: ~83 components
- **Design Tokens**: Yes — CSS-in-JS via styled-components
- **Accessibility**: Core focus — accessibility built into every component
- **Theming**: Granular component customization via theme utility functions
- **Best For**: Customer support interfaces, help desk UIs, service platforms
- **Key Pattern**: Multi-package monorepo architecture for granular dependency management

#### 8. Spectrum — Adobe
- **Site**: https://spectrum.adobe.com/
- **GitHub**: https://github.com/adobe/react-spectrum
- **Framework**: React (React Spectrum), Web Components (Spectrum Web Components)
- **Components**: ~50-62 components
- **Design Tokens**: Yes — full Spectrum color tokens, CSS custom properties
- **Accessibility**: WCAG 2.1 AA+ — **industry-leading** via React Aria (WAI-ARIA Authoring Practices), full i18n
- **Theming**: Light/dark mode with zero extra styling, token customization
- **Best For**: Creative tools, media applications, complex professional interfaces
- **Key Pattern**: Three-layer architecture — React Spectrum (components) → React Aria (a11y hooks) → React Stately (state management). React Aria is reusable independently for any project.

#### 9. Chakra UI — Community
- **Site**: https://chakra-ui.com/
- **GitHub**: https://github.com/chakra-ui/chakra-ui
- **Framework**: React, Next.js RSC; Ark UI (headless: React, Vue, Solid, Svelte)
- **Components**: ~50+ styled components, 45+ headless primitives in Ark UI
- **Design Tokens**: Yes — centralized theme object (colors, spacing, sizes, typography, radii, elevation, motion)
- **Accessibility**: WAI-ARIA compliant, WCAG 2.1 contrast, built-in focus management
- **Theming**: Single theme object, light/dark out of the box, `extendTheme` customization, style props system
- **Best For**: Rapid prototyping, startups, apps needing quick iteration with good defaults
- **Key Pattern**: Composition over configuration — atomic components (Box, Flex, Stack)

#### 10. Carbon — IBM
- **Site**: https://www.carbondesignsystem.com/
- **GitHub**: https://github.com/carbon-design-system
- **Framework**: React (primary), Web Components, Angular, Vue/Svelte (community)
- **Components**: ~50+ production-ready
- **Design Tokens**: Yes — token-based color, type, and spacing systems standardized across themes
- **Accessibility**: WCAG 2.1 AA — IBM Accessibility Checklist (WCAG AA, Section 508, European standards)
- **Theming**: Four built-in themes (White, Gray 10, Gray 90, Gray 100), 16-column grid
- **Best For**: Enterprise software, regulated industries, data-dense business apps
- **Key Pattern**: Design values — Deliberate, Inclusive, Consistent, Humanistic

---

### Tier 3 — Specialized & Growing (11–15)

#### 11. Base Web — Uber
- **Site**: https://base.uber.com/
- **GitHub**: https://github.com/uber/baseweb
- **Framework**: React
- **Components**: ~50-60 components
- **Design Tokens**: Yes — top-level theme entry point for colors, sizing, typography
- **Accessibility**: First-class — keyboard navigation, screen reader compatibility
- **Theming**: Comprehensive theme provider, light/dark, per-component `overrides` pattern
- **Best For**: Ride-sharing/logistics UIs, map-heavy interfaces, multi-product ecosystems
- **Key Pattern**: `overrides` pattern for deep component customization without forking

#### 12. Elastic UI (EUI) — Elastic
- **Site**: https://eui.elastic.co/
- **GitHub**: https://github.com/elastic/eui
- **Framework**: React + TypeScript
- **Components**: 100+ exported components (mature, stable)
- **Design Tokens**: Yes — structured tokens, three core colors + six-level grayscale
- **Accessibility**: WCAG 2.1 — color-blind-safe palettes, tested across assistive technologies
- **Theming**: Themable with minimal code, CSS variable-based
- **Best For**: Data visualization dashboards, search/analytics interfaces, observability tools
- **Key Pattern**: Data-density-first design — optimized for information-rich screens

#### 13. Pajamas — GitLab
- **Site**: https://design.gitlab.com/
- **Repo**: https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com
- **Framework**: Vue.js
- **Accessibility**: WCAG 2.1 AA compliance target
- **Theming**: Token-based with Figma integration
- **Best For**: DevOps platforms, CI/CD interfaces, code management tools
- **Key Pattern**: Open-source design system for open-source product — full transparency in design decisions

#### 14. Vuetify — Community
- **Site**: https://vuetifyjs.com/
- **GitHub**: https://github.com/vuetifyjs/vuetify
- **Framework**: Vue.js 3 (exclusive)
- **Components**: 80-100+ customizable components
- **Design Tokens**: Yes — SASS variables and CSS custom properties
- **Accessibility**: WCAG compliant — ARIA support, keyboard navigation, focus management
- **Theming**: Dynamic theming, light/dark mode, Blueprint system for global defaults, MD3 dynamic color
- **Best For**: Vue.js applications, Material Design-aligned projects, rapid Vue prototyping
- **Key Pattern**: Blueprint system for establishing global component defaults across entire app

#### 15. Mantine — Community
- **Site**: https://mantine.dev/
- **GitHub**: https://github.com/mantinedev/mantine
- **Framework**: React + TypeScript (Next.js, Remix, Vite integrations)
- **Components**: **120+ components and 70+ hooks** (largest component count on this list)
- **Design Tokens**: Yes — color roles, spacing scales, typography, radii, elevation, motion
- **Accessibility**: WCAG adherent — pre-configured ARIA, keyboard navigation, screen reader friendly
- **Theming**: Light/dark out of the box, `createTheme` for full customization, Styles API, CSS modules
- **Best For**: Full-featured React apps, developers wanting maximum components out of the box
- **Key Pattern**: Hooks library (70+) as a standalone value — useForm, useDisclosure, useClipboard, etc.

---

### Tier 4 — Focused Solutions (16–20)

#### 16. Material UI (MUI) — Community
- **Site**: https://mui.com/material-ui/
- **GitHub**: https://github.com/mui
- **Framework**: React (Material UI, Joy UI, Base UI headless)
- **Components**: ~60-70+ core, plus advanced (Data Grid, Date Pickers, Charts) in MUI X
- **Design Tokens**: Yes — `createTheme()`, CSS variables, palette/typography/spacing/breakpoints/shadows/z-index
- **Accessibility**: WCAG 2.1 AA in default theme (some gaps in focus-visible states)
- **Theming**: `ThemeProvider`, light/dark, CSS variables mode, `sx` prop, `styled()` API
- **Best For**: React apps wanting Material Design, rapid enterprise development, teams needing extensive docs
- **Key Pattern**: Three-tier product — Material UI (opinionated) → Joy UI (alternative design) → Base UI (headless)

#### 17. Radix — WorkOS
- **Site**: https://www.radix-ui.com/primitives
- **GitHub**: https://github.com/radix-ui
- **Framework**: React (unstyled primitives)
- **Components**: 30+ primitives (foundation for shadcn/ui)
- **Design Tokens**: Partial (via Radix Themes); Radix Colors provides a11y-guaranteed color scales
- **Accessibility**: WCAG 2.1 + WAI-ARIA Authoring Practices — focus management, keyboard nav, ARIA handled correctly
- **Theming**: CSS variable-based (via Radix Themes layer), bring-your-own-styles for Primitives
- **Best For**: Custom design systems, projects needing full visual control, shadcn/ui-based apps
- **Key Pattern**: Headless/unstyled primitives — maximum design freedom with guaranteed accessibility

#### 18. Blueprint — Palantir
- **Site**: https://blueprintjs.com/
- **GitHub**: https://github.com/palantir/blueprint
- **Framework**: React + TypeScript
- **Components**: ~40-50 core across multiple packages (core, datetime, icons, select, table)
- **Design Tokens**: Yes — SCSS variables for colors, spacing, typography
- **Accessibility**: WCAG 2.0 baseline — colorblindness-safe colors, keyboard navigation
- **Theming**: Dark theme built-in (`.bp5-dark` class), SCSS variable overrides
- **Best For**: Desktop-class data-dense web apps, analytics dashboards, enterprise tools
- **Key Pattern**: Desktop-optimized — designed for complex, data-dense interfaces (not mobile-first)

#### 19. Angular Material — Google
- **Site**: https://material.angular.io/
- **GitHub**: https://github.com/angular/components
- **Framework**: Angular (exclusive)
- **Components**: ~35-40 Material components + ~15 CDK behavioral modules, **800+ design tokens**
- **Design Tokens**: Yes — M3 token-based theming with `mat.theme()` mixin, system-level CSS variables
- **Accessibility**: WCAG 2.1 AA — `mat.strong-focus-indicators()` for 4.5:1 focus visibility, CDK a11y module
- **Theming**: M3-based `mat.theme()`, pre-built + custom themes, color/typography/density dimensions
- **Best For**: Angular applications, enterprise Angular shops, Material Design compliance
- **Key Pattern**: CDK (Component Dev Kit) — behavioral primitives separate from styled components, reusable in custom components

#### 20. Pluralsight Design System — Pluralsight
- **Site**: https://design-system.pluralsight.com/
- **GitHub**: https://github.com/pluralsight/classic-design-system
- **Framework**: React + TypeScript (Classic in maintenance mode, successor is Pando)
- **Design Tokens**: Yes — `design-tokens` package as single source of truth, CSS custom properties
- **Accessibility**: Core priority — Pando was redesigned from scratch to fix Classic's accessibility gaps
- **Theming**: Light/dark/system mode out of the box, token overrides
- **Best For**: EdTech platforms, learning management systems, content delivery interfaces
- **Key Pattern**: Ground-up accessibility redesign — demonstrates how to evolve a design system with a11y as the driver

---

## Component Taxonomy

These 60 component types appear across the top 20 systems (sourced from UI Guideline's cross-system analysis):

### Data Display
Calendar, Table, Carousel, Card, Collapse/Accordion

### Inputs
Search, Number Input, Text Input, Textarea, File Uploader, Date Picker, Select, Combobox

### Overlays
Modal/Dialog, Tooltip, Popover

### Buttons
Button, Toggle Button

### Controls
Color Picker, Rating, Slider, Switch, Checkbox, Radio

### Navigation
Breadcrumbs, Pagination, Link, Stepper, Menu, Tabs, Sidebar

### Notifications
Alert, Toast/Snackbar, Inline Alert

### Loaders
Spinner, Progress Bar, Skeleton

### States
Empty State, Error State, Success State

### Atomic Elements
Divider, Badge, Avatar, Tag/Chip

---

## Planning Decision Framework

When helping a user plan their frontend architecture, use this framework:

### Step 1 — Technology Match
| If the project uses... | Consider these systems first |
|---|---|
| React | MUI, Chakra UI, Mantine, Ant Design, Radix + shadcn/ui |
| Vue | Vuetify, Ant Design Vue, Mantine (React only) |
| Angular | Angular Material, Ant Design (NG-ZORRO) |
| Framework-agnostic | Material Design (Web Components), Polaris, Spectrum Web Components |
| Multiple platforms | Material Design, Fluent 2, Carbon |

### Step 2 — Use Case Match
| If the project is... | Look at patterns from |
|---|---|
| E-commerce / SaaS admin | Polaris (Shopify), Ant Design |
| Enterprise / data-dense | Carbon (IBM), Blueprint (Palantir), Elastic UI |
| Developer tools | Primer (GitHub), Pajamas (GitLab) |
| Creative / media tools | Spectrum (Adobe) |
| Customer support | Garden (Zendesk) |
| Cross-platform | Material Design, Fluent 2 |
| Rapid prototyping | Chakra UI, Mantine |
| Custom design (unstyled) | Radix, React Aria (from Spectrum) |
| EdTech / learning | Pluralsight, Carbon |
| Logistics / maps | Base Web (Uber) |

### Step 3 — Architecture Decisions

**Design Tokens Strategy** — All 20 systems now use design tokens. Recommend:
- Two-layer token system (global/primitive → semantic/alias) — used by Fluent 2, Angular Material
- Three-layer token system (reference → system → component) — used by Material Design
- CSS custom properties as the transport layer — universal pattern

**Accessibility Baseline** — Recommend WCAG 2.1 AA minimum:
- Use React Aria (from Adobe Spectrum) for accessible hooks in custom components
- Use Radix Primitives for accessible unstyled components
- Reference Primer's 9-mode accessibility system for comprehensive theme support

**Theming Architecture** — Common proven patterns:
- Token-based theming with CSS custom properties (most systems)
- ThemeProvider context pattern (Chakra, MUI, Carbon, Mantine)
- Class-based theme switching (Blueprint, Primer CSS)

**Component API Patterns** — Proven approaches:
- Composition pattern: `<Card><Card.Header /><Card.Body /></Card>` (Chakra, Mantine, MUI)
- Override pattern: `overrides` prop for deep customization (Base Web/Uber)
- Slot pattern: Named slots for content injection (Spectrum, Fluent)
- Headless pattern: Behavior without styles (Radix, React Aria, Base UI)

---

## Quick Reference Links

| # | System | GitHub | Docs |
|---|---|---|---|
| 1 | Material Design | [material-components](https://github.com/material-components) | [m3.material.io](https://m3.material.io/) |
| 2 | Atlassian | [Bitbucket](https://bitbucket.org/atlassian/atlassian-frontend-mirror) | [atlassian.design](https://atlassian.design/) |
| 3 | Polaris | [Shopify/polaris](https://github.com/Shopify/polaris) | [polaris.shopify.com](https://polaris.shopify.com/) |
| 4 | Ant Design | [ant-design](https://github.com/ant-design/ant-design) | [ant.design](https://ant.design/) |
| 5 | Fluent 2 | [microsoft/fluentui](https://github.com/microsoft/fluentui) | [fluent2.microsoft.design](https://fluent2.microsoft.design/) |
| 6 | Primer | [primer](https://github.com/primer) | [primer.style](https://primer.style/) |
| 7 | Garden | [zendeskgarden](https://github.com/zendeskgarden) | [garden.zendesk.com](https://garden.zendesk.com/) |
| 8 | Spectrum | [adobe/react-spectrum](https://github.com/adobe/react-spectrum) | [spectrum.adobe.com](https://spectrum.adobe.com/) |
| 9 | Chakra UI | [chakra-ui](https://github.com/chakra-ui/chakra-ui) | [chakra-ui.com](https://chakra-ui.com/) |
| 10 | Carbon | [carbon-design-system](https://github.com/carbon-design-system) | [carbondesignsystem.com](https://www.carbondesignsystem.com/) |
| 11 | Base Web | [uber/baseweb](https://github.com/uber/baseweb) | [base.uber.com](https://base.uber.com/) |
| 12 | Elastic UI | [elastic/eui](https://github.com/elastic/eui) | [eui.elastic.co](https://eui.elastic.co/) |
| 13 | Pajamas | [GitLab](https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com) | [design.gitlab.com](https://design.gitlab.com/) |
| 14 | Vuetify | [vuetifyjs/vuetify](https://github.com/vuetifyjs/vuetify) | [vuetifyjs.com](https://vuetifyjs.com/) |
| 15 | Mantine | [mantinedev/mantine](https://github.com/mantinedev/mantine) | [mantine.dev](https://mantine.dev/) |
| 16 | Material UI | [mui](https://github.com/mui) | [mui.com](https://mui.com/material-ui/) |
| 17 | Radix | [radix-ui](https://github.com/radix-ui) | [radix-ui.com](https://www.radix-ui.com/) |
| 18 | Blueprint | [palantir/blueprint](https://github.com/palantir/blueprint) | [blueprintjs.com](https://blueprintjs.com/) |
| 19 | Angular Material | [angular/components](https://github.com/angular/components) | [material.angular.io](https://material.angular.io/) |
| 20 | Pluralsight | [pluralsight/classic-design-system](https://github.com/pluralsight/classic-design-system) | [design-system.pluralsight.com](https://design-system.pluralsight.com/) |

---

*Data sourced from [uiguideline.com](https://www.uiguideline.com) and the official GitHub repositories of each design system.*
