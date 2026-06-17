# Architecture

## Organization

The site is organized by research theme first.

```text
docs/
  themes/
    analyst/
      ideas/
      papers/
      sellside_reports/
      factor_notes/
      experiments/
```

Each research theme can reuse the same internal structure:

- `ideas/`: raw hypotheses and research directions.
- `papers/`: academic paper notes.
- `sellside_reports/`: sell-side report notes.
- `factor_notes/`: cleaned factor definitions and implementation-ready notes.
- `experiments/`: experiment logs, backtest summaries, and reproducibility notes.

## Conventions

Use stable English directory names and readable Markdown titles.

Keep daily notes under `daily/`. Use them for chronological capture, then promote durable material into the relevant research theme.

Keep cross-theme material under `references/`.
