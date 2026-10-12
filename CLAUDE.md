# Futures Trade Calculator

Static single-file site (`index.html`), hosted on GitHub Pages from `main` / root. No build step, no external scripts.

## Design System
Follow `apple-design-system-analysis.md` (Apple style). Key rules:

- **Colors:** use the CSS tokens on `:root` only. Neutral base (`#f5f5f7` bg, `#ffffff` cards, `#1d1d1f` text, `#6e6e73` muted, `#d2d2d7` border). `#0071e3` is the only accent, used for primary actions and focus. Exception: green/red/orange are allowed only for LONG/SHORT, profit/loss and warnings.
- **Dark mode:** `#000000` bg, `#1d1d1f` cards, `#f5f5f7` text, redefined under `prefers-color-scheme: dark`.
- **Type:** SF Pro system stack (no web fonts). Display 56px/600, H2 21px/600, body 17px/400, labels 14px, captions 12px minimum. Headings use 600, body uses 400. Numbers use `tabular-nums`.
- **Radius:** only `8px` (inputs), `11px` (cards), `9999px` (buttons/segmented controls).
- **Depth:** flat, no `box-shadow` on UI. Separate content with whitespace and background, not borders (thin `--border` rules are OK inside result lists).
- **Spacing:** 4px scale `[4, 8, 12, 16, 20, 24, 32, 48, 128]`.
- **Focus:** `2px solid #0071e3` outline with `3px` offset on every interactive element.
- **Motion:** `320ms cubic-bezier(0.4, 0, 0.6, 1)`.
- **Layout:** max-width 980px, sticky 44px blurred nav, single column at `max-width: 734px`, touch targets ≥ 44px where possible.
- **Language:** UI copy is Thai.
