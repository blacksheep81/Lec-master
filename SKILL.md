---
name: lec-master
description: Turn lecture slides or PDFs plus transcript/subtitle TXT files into accurate, exam-oriented study notes. Use for lecture summaries, course revision packs, key-point notes, formula sheets, teacher emphasis, worked examples, or multi-week revision websites.
---

# Lecture Revision

Use supplied course materials as the source of truth. Do not invent content absent from the slides or transcript; label reasonable inferences explicitly.

## Workflow

1. Inventory and pair files by week, lecture, or topic when filenames allow. Recognize PDF, PPT/PPTX, TXT, subtitle, image, tutorial, and solution files.
2. Extract content while preserving slide/page numbers. Render pages when diagrams, layout, handwriting, or formulas matter. Read transcripts fully and retain timestamps or section markers.
3. Align transcript explanations to the relevant slide/page/topic. Use transcripts for intuition, teacher emphasis, worked reasoning, warnings, and exam cues; use slides for formal definitions, notation, formulas, diagrams, and stated examples.
4. Produce: learning objectives and big picture; concepts and definitions; formulas with symbols, assumptions, and use cases; step-by-step methods; worked examples; common mistakes and edge cases; teacher emphasis; final checklist; and self-test questions.
5. Cite evidence inline as `(Slide 4)`, `(PDF p. 7)`, or `(Transcript 12:30–13:10)`. If evidence cannot be located, write `source not located` instead of fabricating a citation.
6. Match the requested output. Default to Markdown notes. For multiple lectures, add a cross-lecture glossary, formula sheet, and prerequisite/dependency map. For a requested PDF or website, create it and verify the rendered result.

## Subject guidance

- Statistics/mathematics: distinguish definitions, conditions, statistics/estimators, distributions, assumptions, and interpretations. Check dimensions, signs, and limiting cases in formulas.
- Programming/practical lectures: separate concepts, syntax/APIs, execution steps, examples, and debugging pitfalls. Do not claim code was run unless tested.
- Diagrams/tables: describe relationships in text and retain their source reference.

## Quality checks

- Every major claim, formula, and exam cue has a nearby source reference or an inference label.
- Notation stays consistent with the source; define renamed or normalized notation.
- Transcript-only explanations are not presented as official slide content.
- Remove duplication without losing qualifications or exceptions.
- End with missing, ambiguous, or unreadable source material.
- For paired sources, verify that a slide claim carries its page and an oral clarification carries its timestamp. If the transcript contradicts the slide, report both claims and their locations before choosing a study note. If the user wants the PDF-first LaTeX cheat-sheet workflow, prefer `summarize-slides` when installed. Use this skill for Markdown-first notes and cross-lecture synthesis.

## Default output order

Big picture → Concepts → Formulas → Methods → Examples → Pitfalls → Exam cues → Self-test → Sources and missing material.
