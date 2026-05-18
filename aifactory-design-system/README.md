# AIFactory Design System

A modular CSS design system extracted from the AIFactory competition platform. Split into four concern-separated layers so you can load only what you need.

## Files

| File | Purpose |
|------|---------|
| `tokens.css` | Core design tokens: color palette, typography scale, line heights, border radius, shadows |
| `tokens.web.css` | Web layout tokens: sticky element heights, top offsets, container width, breakpoint reference |
| `components.css` | Base components: reset, `.btn`, `.tag`, `.badge`, headings, `.body-txt`, callouts, grids, data table, stat cards, segmented control, TOC links |
| `components.web.css` | Full-page layout components: navbar, hero, tab nav, status bar, sidebar, leaderboard, discussion, team search, FAQ, code blocks, responsive rules |
| `doc.css` | Documentation/reference stylesheet (used by reference.html) |
| `reference.html` | Living component reference page |
| `assets/AIFactory.svg` | Primary AIFactory logotype (dark) |
| `assets/Yellowlogo.svg` | AIFactory logotype (amber/yellow variant) |

## Usage

Load files in this order:

```html
<link rel="stylesheet" href="tokens.css">
<link rel="stylesheet" href="tokens.web.css">   <!-- omit for non-web contexts -->
<link rel="stylesheet" href="components.css">
<link rel="stylesheet" href="components.web.css"> <!-- omit for non-full-page contexts -->
```

## Breakpoints

| Name | Width | Notes |
|------|-------|-------|
| sm | 640px | Small tablets |
| md | 768px | Tablets |
| lg | 1024px | Desktop divider — mobile/desktop split |
| xl | 1280px | Wide desktop |

The `@media (max-width:1024px)` and `@media (max-width:480px)` blocks in `components.web.css` handle all responsive behaviour.

## Font

Uses **Pretendard Variable** with system fallbacks. Load from CDN or self-host:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/variable/pretendardvariable.css">
```
