# Agent Instructions

## Project Context

Repo holds course material for Automatic Image Analysis + LaTeX script project in
`Script/`. Script = explanatory learning document, not plain summary.

Script explains lectures (`Lectures/`), but every chapter must also cover
matching exercises (`Exercises/`) and exam tasks (`Exams/`). Goal: reader can
solve exam and exercise questions after studying script. When writing or
revising chapter, check which exercise/exam tasks touch its topics. Ensure script
covers concepts, formulas, and worked reasoning needed to solve them.

Exam/exercise tasks only loosely tied to lectures go into appendix
(`Script/appendix_supplements.tex`), not forced into chapter story. Rule: topic
appears in exercises/exams but barely or not in lectures, and fits scope of
existing chapters (e.g. edge detection, Fourier transform and descriptors,
classical classifiers, Hough forest, DPM). Keep each appendix unit brief and
limited to necessary knowledge: broad intuition of domain first, then specific
thing exams ask, then knowledge required to solve it. Chapter text links to
appendix with one pointer sentence. Tasks belonging to later lectures (e.g. CNN
arithmetic, Bayes, RNN) wait for their own chapter, not appendix.

## LaTeX Script Preferences

- Compile only one PDF: `Script/main.pdf`.
- Keep `Script/main.tex` as root LaTeX document.
- Put larger chapter/unit bodies in separate `.tex` files, include from
  `main.tex` with `\input{...}`. No own preamble in included files, no separate
  PDFs for them.
- Keep section hierarchy restrained. Top-level sections = real chapters or major
  units. Inside chapter/unit, use `\subsection{...}` for meaningful blocks, each
  substantial enough to keep reading flow. No new subsection after only one
  short paragraph; merge related points into larger subsection.
- Never place `\section{...}` directly before `\subsection{...}`, or one
  `\subsection{...}` directly before another heading. Add orienting text between
  headings, or remove/merge one heading.
- No placeholder-only prose. New material needs enough substance to be useful on
  its own.

## Teaching Style

- Explanatory, direct style, useful for studying.
- No meta-references to document as script, lecture, lecture notes, or
  lecture-based material. Present course contents directly.
- Intuitive explanation before formal notation.
- Use figures, schematic diagrams, tables, equations to make concepts concrete.

## Visuals And Math

- Diagram labels clear, separated from boxes and arrows. Check for overlapping
  labels before finishing.
- Figures compact enough to fit text width, no overfull boxes.
- Tables for comparisons, taxonomies, practical checklists.
- Include formulas when they clarify concept: image formation, Bayesian
  inference, convolution, camera projection, training objectives.
- Every figure and table gets short explanatory caption.
- When prose resumes right after displayed formula, figure, table, or list
  environment, use `\noindent` so continuation has no paragraph indent.

## Build And Verification

- Build from `Script/` with:

  ```bash
  make TEX=/c/texlive/2026/bin/windows/pdflatex.exe
  ```

- Run `make clean` after successful builds to remove LaTeX auxiliary files.
- When adding included `.tex` files or figure assets, update `Script/Makefile`
  so changes trigger rebuild.
- No stale separate PDFs for included sections.
