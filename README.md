# CSS-First Agent Skill

> Transform any AI agent into a CSS-first expert. Zero-JavaScript solutions using cutting-edge CSS features (2021-2026).

## What It Does

This skill gives AI agents deep knowledge of modern CSS so they provide CSS-only solutions instead of reaching for JavaScript. It includes:

- **7 behavioral rules** — CSS-only enforcement, logical properties, modern features, semantic intent analysis, framework detection, browser support, progressive enhancement
- **57 production-ready CSS demos** — layout, responsive, container queries, animation, theming, positioning, interaction, visual, specificity, functions & values
- **Live MDN integration** — fetch current Baseline status and browser support data on demand

## Features

| Capability                  | Description                                                                                             |
| --------------------------- | ------------------------------------------------------------------------------------------------------- |
| Semantic Intent Recognition | Detects layout, animation, spacing, responsive, visual, and interaction intents                         |
| Framework Detection         | Auto-detects React, Vue, Angular, Svelte, Tailwind, Bootstrap                                           |
| Logical Properties First    | Prioritizes `inline-size`, `margin-inline`, etc. for internationalization                               |
| Modern CSS (2021-2026)      | Container queries (incl. name-only), view transitions, scroll-driven/triggered animations, `light-dark()`, anchor positioning, `@layer`, `@scope`, `revert-rule`, `if()`, `@function`, advanced `attr()`, `contrast-color()`, grid lanes, gap decorations, `shape-outside` shapes |
| Browser Support Awareness   | Every suggestion includes Baseline status (Widely Available / Newly Available / Limited / Experimental) |
| Progressive Enhancement     | Core functionality first, enhancements layered with `@supports`                                         |

## Quick Reference

| Status | User Intent          | CSS Solution                    | Demo                                              |
| :----: | -------------------- | ------------------------------- | ------------------------------------------------- |
| 🟢 | Center element       | Flexbox / Grid                  | `css-demos/layout/centering-logical.css`          |
| 🟢 | Aligned grids        | Subgrid                         | `css-demos/layout/subgrid.css`                    |
| 🔵 | Parent selection     | `:has()`                        | `css-demos/layout/has-selector.css`               |
| 🔵 | Component styles     | CSS Nesting                     | `css-demos/layout/css-nesting.css`                |
| 🟣 | Masonry layout       | Grid Lanes                      | `css-demos/layout/grid-lanes-masonry.css`         |
| 🟢 | Responsive layout    | Media queries (range syntax)    | `css-demos/responsive/media-queries.css`          |
| 🟢 | Feature detection    | `@supports`                     | `css-demos/responsive/supports-rule.css`          |
| 🟢 | Container responsive | Container size queries          | `css-demos/container/size-queries.css`            |
| 🟡 | Component theming    | Container style queries         | `css-demos/container/style-queries.css`           |
| 🟣 | Sticky detection     | Scroll state queries            | `css-demos/container/scroll-state-queries.css`    |
| 🟣 | Tooltip arrow flip   | Anchored container queries      | `css-demos/container/anchored-queries.css`        |
| 🟣 | Container by name    | `@container` name without type  | `css-demos/container/named-queries.css`           |
| 🔵 | Dark mode            | `light-dark()`                  | `css-demos/theming/light-dark-function.css`       |
| 🔵 | Page transitions     | View Transitions (+ element-scoped) | `css-demos/animation/view-transitions.css`   |
| 🟡 | Scroll effects       | Scroll-driven animations        | `css-demos/animation/scroll-driven.css`           |
| 🟣 | Scroll reveals       | Scroll-triggered animations     | `css-demos/animation/scroll-triggered.css`        |
| 🔵 | Entry/exit animation | `@starting-style`               | `css-demos/animation/starting-style.css`          |
| 🟡 | Tooltips             | Anchor Positioning              | `css-demos/positioning/anchor-positioning.css`    |
| 🟣 | Carousel / Tabs      | CSS Carousel                    | `css-demos/interaction/css-carousel.css`          |
| 🔵 | Popovers / Dropdowns | Popover API                     | `css-demos/interaction/popover.css`               |
| 🟢 | Touch vs pointer     | Hover media queries             | `css-demos/interaction/hover-media-queries.css`   |
| 🟢 | Form validation      | `:user-valid` / `:user-invalid` | `css-demos/visual/form-validation.css`            |
| 🟢 | Color variations     | `color-mix()`                   | `css-demos/visual/color-mix.css`                  |
| 🟣 | Modern shapes        | `corner-shape`                  | `css-demos/visual/corner-shape.css`               |
| 🟣 | Text wrap around shapes | `shape-outside` shape functions | `css-demos/visual/shape-outside-functions.css` |
| 🔵 | Underline ink skipping | `text-decoration-skip-ink`    | `css-demos/visual/text-decoration-skip-ink.css`   |
| 🔵 | Crisp pixel-art scaling | `image-rendering: crisp-edges` | `css-demos/visual/image-rendering.css`          |
| 🟢 | Aligned / steady digits | `font-variant-numeric: tabular-nums` | `css-demos/visual/font-variant-numeric.css` |
| 🟣 | Conditional values   | `if()`                          | `css-demos/functions/css-if-function.css`         |
| 🟣 | Reusable logic       | `@function`                     | `css-demos/functions/custom-functions.css`        |
| 🟣 | Data-driven styles   | Advanced `attr()`               | `css-demos/functions/advanced-attr.css`           |
| 🔵 | Auto contrast text   | `contrast-color()`              | `css-demos/functions/contrast-color.css`          |
| 🟢 | Cascade control      | `@layer`                        | `css-demos/specificity/cascade-layers.css`        |
| 🔵 | Scoped styles        | `@scope`                        | `css-demos/specificity/scope-rule.css`            |
| 🟣 | Roll back one rule   | `revert-rule`                   | `css-demos/specificity/revert-rule.css`           |

## Structure

```
SKILL.md                          # Skill definition (loaded by agents)
references/
  rules/                          # 7 behavioral rules
  live-mdn-fetch.md               # Live MDN data fetch workflow
css-demos/
  INDEX.md                        # Full catalog with MDN links & baseline status
  layout/                         # Centering, spacing, subgrid, :has(), nesting, grid lanes
  responsive/                     # Media queries (range syntax), @supports
  container/                      # Size, style, scroll-state, anchored, name-only queries
  animation/                      # View transitions, scroll-driven, scroll-triggered, @starting-style
  theming/                        # Dark mode with light-dark()
  positioning/                    # Anchor positioning
  interaction/                    # CSS Carousel, popover, hover media queries
  visual/                         # Form validation, color-mix(), corner-shape
  functions/                      # if(), @function, advanced attr(), contrast-color()
  specificity/                    # @layer cascade layers, @scope scoped styles
```

## Baseline Status Indicators

- **🟢 Widely Available** (95%+) — safe for production
- **🔵 Newly Available** (85-94%) — recently stable, verify target browsers
- **🟡 Limited Availability** (70-84%) — use with progressive enhancement
- **🟣 Experimental** (<70%) — cutting-edge, use cautiously

## License

MIT
