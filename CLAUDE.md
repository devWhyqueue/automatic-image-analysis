# Agent Instructions

## Project Context

This repository contains course material for Automatic Image Analysis and a
LaTeX script project in `Script/`. The script should become an explanatory
learning document, not just a plain summary.

The script explains the lectures (`Lectures/`), but every chapter must also
take the corresponding exercises (`Exercises/`) and exam tasks (`Exams/`) into
account. The overarching goal is that a reader can successfully solve exam and
exercise questions after studying the script. When writing or revising a
chapter, check which exercise and exam tasks touch its topics, and make sure the
script covers the concepts, formulas, and worked reasoning needed to solve them.

## LaTeX Script Preferences

- Compile only one PDF output for the script: `Script/main.pdf`.
- Keep `Script/main.tex` as the root LaTeX document.
- Put larger chapter or unit bodies in separate `.tex` files, then include
  them from `main.tex` with `\input{...}`. Do not give included files their own
  document preamble or compile them into separate PDFs.
- Keep section hierarchy restrained. Use top-level sections for real document
  chapters or major units. Inside a chapter or unit, use `\subsection{...}` for
  meaningful blocks, but keep each subsection substantial enough to preserve
  reading flow. Do not create a new subsection after only one short paragraph;
  combine closely related points into a larger subsection instead.
- Never place a `\section{...}` directly before a `\subsection{...}`, or one
  `\subsection{...}` directly before another heading. Add meaningful orienting
  text between headings, or remove/merge one of the headings.
- Avoid placeholder-only prose. When adding material, include enough substance
  that the section is useful on its own.

## Teaching Style

- Write in an explanatory, direct style that is useful for studying.
- Avoid meta-references to the document as a script, lecture, lecture notes, or
  material based on a lecture. Present the course contents directly.
- Prefer intuitive explanations before formal notation.
- Use figures, schematic diagrams, tables, and equations to make concepts more
  concrete.
- Avoid overly dense generated infographics. Prefer simple, local TikZ diagrams
  that explain one idea clearly.

## Visuals And Math

- Use TikZ for simple conceptual diagrams such as pipelines, ambiguity examples,
  task taxonomies, and evaluation flows.
- Keep diagram labels clear and separated from boxes and arrows. Check for
  overlapping labels before finishing.
- Keep figures compact enough to fit the text width without overfull boxes.
- Use tables for comparisons, taxonomies, and practical checklists.
- Include formulas when they clarify the concept, such as image formation,
  Bayesian inference, convolution, camera projection, and training objectives.
- Every figure and table should have a short explanatory caption.
- When prose resumes immediately after a displayed formula, figure, table, or
  list environment, use `\noindent` so the continuation does not start with a
  paragraph indent.

## Build And Verification

- Build from `Script/` with:

  ```bash
  make TEX=/c/texlive/2026/bin/windows/pdflatex.exe
  ```

- Run `make clean` after successful builds to remove LaTeX auxiliary files.
- If included `.tex` files or figure assets are added, update `Script/Makefile`
  so changes trigger a rebuild.
- Do not leave stale separate PDFs for included sections.
