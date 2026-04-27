# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when
working with code in this repository.

## What This Is

A study repository for probability and statistics, following Harvard's
Stat 110 curriculum (stat110.net). Content lives in Emacs org-mode
files (`.org`) with embedded Python code blocks for worked examples.

## Workflow

All content is authored in Emacs org-mode. Python code blocks are
executed interactively with `C-c C-c` inside Emacs. LaTeX math
previews render via `M-x org-latex-preview`.

To run Python snippets outside Emacs, extract and run with `python3`
directly — all examples use only the standard library (`math`,
`itertools`, `collections`).

## File Layout

- `ch00_summary_glossary.org` — course outline and glossary
- `ch01_prob_and_counting.org` — chapter notes
- `lectures/` — raw lecture notes
- `exercises/` — problem sets with worked Python solutions
- `ltximg/` — auto-generated LaTeX SVG cache (do not edit manually)

## Org-mode Conventions

Files use this header for Python blocks:
```
#+PROPERTY: header-args:python :session *Python* :results output :exports both
#+STARTUP: latexpreview
```

Math is written inline with LaTeX (`\(...\)`) or in equation blocks (`\begin{equation}...\end{equation}`).
