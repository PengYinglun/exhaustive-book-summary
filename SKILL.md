---
name: exhaustive-book-summary
description: "Produce an exhaustive, high-fidelity analysis of an entire user-provided book as one unified, professionally formatted DOCX. Use when the user uploads or identifies a book and requests a comprehensive summary, complete book analysis, chapter-by-chapter treatment, or invokes $exhaustive-book-summary, including short prompts containing only title and author. Support PDF, EPUB, DOCX, scanned pages, and other readable book files. Audit source completeness, preserve every unique substantive claim and example while compressing repetition, separate book-derived analysis from independent critique, and include a separately sourced external critical assessment. Never substitute reviews, web summaries, memory, or outside material for an inaccessible book."
---

# Exhaustive Book Summary

Treat a message containing only these fields as a complete request to run this workflow on the matching accessible book:

```text
Book name: <title>
Author: <author>
```

Accept minor variations, missing punctuation, or reversed field order. Use edition, translator, and publication year when provided. Do not require the user to repeat the workflow instructions.

## Outcome contract

- Produce one unified, downloadable DOCX containing the complete analysis. Use chat only for concise progress updates and the final handoff.
- Do not expose partial chapter installments as the deliverable and do not require the user to type “continue.” Work autonomously through the entire accessible book.
- If DOCX creation is genuinely unavailable, create one persistent, unified artifact in the best available document format rather than splitting the analysis across chat messages.
- Preserve every unique substantive claim, argument, qualification, study, framework, conclusion, and analytically meaningful example. Compress repetition, rhetorical flourish, and decorative narrative detail.
- Keep the faithful book analysis and outside research visibly separate so external material never silently changes the author’s argument.

## 1. Resolve the source

1. Locate the matching book in the current conversation, accessible Library, or user-provided files. Use the relevant Library and file-format skills when applicable.
2. If exactly one accessible file clearly matches, proceed without confirmation. If several editions or files could materially change the analysis, ask the user to identify the intended source.
3. If the book is unavailable, stop and ask the user to upload it. Never replace the book with model memory, reviews, online excerpts, commercial summaries, or outside research.
4. Use edition-specific details from the selected file. Record the exact source filename, edition information when available, file page count, and printed-page range. If the upload has an opaque machine-generated filename, lead with the bibliographic identity and confine that filename to a technical source note.

## 2. Audit coverage before summarizing

Inspect the entire file before substantive drafting, including cover and publication data, table of contents, preface or introduction, every chapter and major section, conclusion or epilogue, appendices, notes, glossary, bibliography, exhibits, and substantively relevant back matter.

Build an internal coverage ledger from the actual source structure. For each item record:

- section or chapter title and order;
- file-page and printed-page range when available;
- extraction or OCR status;
- missing, duplicated, out-of-order, blank, cropped, or illegible content; and
- whether the item has been analyzed and included in the final document.

Distinguish intentionally blank pages and publication artifacts from genuine gaps. Never reconstruct missing text silently.

If a gap materially prevents faithful whole-book analysis, report its exact location and ask for a complete or clearer copy. If a limited gap does not undermine the analysis, state it prominently and continue only with accessible material.

## 3. Analyze in separate passes

Complete these passes before final synthesis:

1. **Structure pass:** map the book’s parts, chapters, chronology, terminology, thesis progression, and conclusion.
2. **Claim-and-evidence pass:** capture every unique substantive claim, supporting argument, study, data point, historical event, example, case, qualification, exception, counterargument, and change in position.
3. **Synthesis pass:** trace cross-chapter themes, causal links, tensions, dependencies, repeated motifs, unresolved questions, and practical implications.

For literary or narrative works, adapt “claim” and “argument” to narrative structure, character development, themes, symbolism, voice, historical context, and interpretive tensions. Do not force an argumentative template where it does not fit.

## 4. Maintain analytical fidelity

- Distinguish the author’s claims, evidence cited by the author, views attributed to others, and the assistant’s analysis.
- Preserve uncertainty, nuance, internal disagreement, qualifications, exceptions, and changes in the author’s position.
- Explain reasoning rather than listing conclusions without their support.
- Do not invent connective logic, evidence, page content, or missing material.
- Paraphrase instead of reproducing long passages. Quote only briefly when exact wording is analytically necessary.
- Give chapter and page references whenever the source supports them. For unpaginated sources, use chapter, section, location, or another stable locator.
- Label uncertain interpretations explicitly.
- Preserve chapter boundaries unless combining sections cannot lose meaningful information.

## 5. Research the external critical assessment

Complete the book-only analysis before beginning outside research. Then research the book’s major claims, contribution, reception, limitations, and continuing relevance using current external sources.

Prioritize sources in this order:

1. peer-reviewed research, systematic reviews, meta-analyses, and replication studies;
2. official datasets, primary historical materials, and authoritative institutional publications;
3. scholarly books, academic reference works, and high-quality specialist synthesis; and
4. reputable secondary sources only when needed for context.

Exclude generic reviews as evidence for substantive claims, along with commercial book summaries, unsourced commentary, and material that merely repeats the book. Scholarly or professional reviews may be used narrowly to document reception, not to validate factual claims. For science or social-science claims, assess whether later evidence supports, narrows, disputes, or supersedes the author’s treatment. For history, philosophy, literature, and classics, use appropriate scholarship and competing interpretations rather than forcing scientific verification.

Date-stamp the research cutoff. Cite every external factual claim and link directly to the supporting source. State when the relevant evidence is mixed, limited, contested, or unavailable. If external research tools are unavailable, disclose that limitation and do not fabricate the section’s evidence.

## 6. Build the unified document

Use the book’s structure and terminology while organizing the DOCX under these sections:

### A. Source and coverage statement

Identify the source edition/file, its apparent completeness, page-count reconciliation, OCR limitations, and the structure covered.

### B. Executive overview

Explain the central thesis or purpose, principal conclusions, intended audience, contribution, and the most important qualifications.

### C. Argument or narrative map

Show how the major claims, evidence, qualifications, conclusions, narrative developments, or thematic arcs connect. Use a structured outline or a compact diagram only when it improves comprehension.

### D. Chapter-by-chapter analysis

For every chapter or major section, explain:

- its purpose and role in the whole book;
- every major claim, development, and supporting line of reasoning;
- important studies, data, evidence, examples, anecdotes, and cases;
- concepts, definitions, distinctions, models, and frameworks;
- assumptions, qualifications, limitations, exceptions, and counterarguments;
- connections with earlier and later sections; and
- changes or developments in the author’s position.

### E. Major themes and concepts

Synthesize recurring ideas across the book and explain how they develop, interact, reinforce one another, or create tensions.

### F. Evidence and examples

Consolidate the most important studies, events, data points, cases, comparisons, and practical examples. Explain what each is intended to demonstrate and the limitations acknowledged in the book.

### G. Conclusions and applications

Present the author’s conclusions, recommendations, predictions, proposed actions, and practical implications. Label the assistant’s extensions or real-world applications as inference.

### H. Critical assessment — book-internal analysis

Clearly label this as independent analysis based only on the supplied book. Evaluate the strongest contributions, weakest or least-supported claims, assumptions, biases, contradictions, unresolved questions, evidentiary gaps, and reasonable counterarguments.

### I. External critical assessment and current research

Keep this subsection separate from the faithful summary. Compare the book’s important claims and contribution with the outside research gathered in Step 5. Explain what has held up, what requires qualification, what later evidence challenges, and what has changed since publication. Include inline citations and a consolidated external source list.

### J. Comprehensive reference section

Provide a glossary, principal frameworks and models, consolidated major conclusions, detailed “what to remember” checklist, and a chapter coverage matrix showing that every source section was included.

## 7. Format and verify the DOCX

Use the document-creation skill and its render-and-verify workflow. Create a readable hierarchy, restrained professional styling, page numbers, a table of contents when practical, stable headings, well-formatted tables, and accessible links/citations. Keep long analytical passages readable without turning the document into a slide deck.

Before delivery, verify all of the following:

- the chapter count and order match the audited source;
- every ledger item is represented in the document or explicitly marked inaccessible;
- no later chapter is compressed merely because the document is long;
- page/chapter references are valid and external citations resolve;
- book-derived analysis and external research are unmistakably separated;
- the DOCX contains no placeholders, truncated sections, repeated installments, or missing cross-references;
- the document opens, renders, and has no clipped tables, orphaned headings, or unreadable pages; and
- the final coverage matrix is complete.

## 8. Deliver concisely in chat

Return only:

- the source-completeness result;
- the central thesis and a few highest-value conclusions;
- any material limitation;
- a brief note on what the external assessment changed or qualified; and
- a link to the unified DOCX.

Do not paste the complete analysis into chat unless the user explicitly asks for it.
