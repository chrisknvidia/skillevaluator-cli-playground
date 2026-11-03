---
name: glossary-builder
description: Builds a small glossary from supplied prose. Use when a reader needs definitions grounded in the text and ambiguous terms identified.
license: MIT
metadata:
  author: SkillEvaluator CI Demo Authors <ci-demo@example.com>
  version: 1.0.0
  tags:
    - demonstration
    - text-assistance
---

# Glossary Builder

## Purpose
Explain specialized terms using only definitions supported by supplied prose.

## Prerequisites
Provide readable source text and, optionally, the intended audience.
No external lookup, software dependencies, or credentials are required.

## Instructions
1. Read the source and identify terms that need explanation for the stated audience.
2. Capture explicit definitions and the sentence that supports each definition.
3. Expand abbreviations only when the expansion appears in the source.
4. Mark an undefined term as “Definition not supplied.”
5. Keep distinct meanings separate when the same term is used in different contexts.
6. Sort terms alphabetically without changing their original spelling.
7. Validate each definition against its supporting sentence.

## Output
Return a Markdown table with Term, Definition, and Source wording columns.
Place ambiguous or undefined terms in a short Follow-up questions list.
If there are no specialized terms, state that no glossary entries are needed.

## Examples
Input:
```text
A batch is a set of requests processed together. Each batch receives a tracking code.
```
Output:
```text
Term: Batch
Definition: A set of requests processed together.
Source wording: A batch is a set of requests processed together.
```
“Tracking code” remains undefined unless the source explains its meaning.

## Limitations
This skill is a reading aid rather than an authoritative dictionary.
It does not introduce external definitions or resolve domain disagreements by guessing.

## Troubleshooting
If the source contains conflicting definitions, include each meaning with its own wording.
If text is empty or invalid, identify the input problem and request a readable excerpt.
