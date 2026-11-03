---
name: evidence-table
description: Organizes supplied claims and observations into an evidence table. Use when a review must distinguish support, uncertainty, and missing proof.
license: MIT
metadata:
  author: SkillEvaluator CI Demo Authors <ci-demo@example.com>
  version: 1.0.0
  tags:
    - demonstration
    - text-assistance
---

# Evidence Table

## Purpose
Make the relationship between a claim and its supplied evidence easy to inspect.

## Prerequisites
Provide the claims and the observations or source excerpts available for review.
No external search, accounts, credentials, or file modifications are required.

## Instructions
1. Separate each factual claim from recommendations and opinions.
2. Match the claim to the exact observation that supports it.
3. Classify support as Supported, Partially supported, Contradicted, or Unverified.
4. Use Supported only when the evidence covers the entire claim.
5. Record scope limits such as a single example or a simulated run.
6. State the smallest additional observation needed to close each proof gap.
7. Validate that no row converts an assumption into an observed fact.

## Output
Return a Markdown table with Claim, Evidence, Support, and Remaining gap columns.
Follow it with at most three questions needed to resolve important gaps.
If no evidence is supplied, label all factual claims Unverified.

## Examples
Input:
```text
Claim: Every export format works.
Observation: A CSV export opened successfully. No other format was checked.
```
Output:
```text
Claim: Every export format works.
Evidence: One CSV export opened successfully.
Support: Partially supported.
Remaining gap: Verify the other promised formats and relevant options.
```
The successful CSV observation does not establish behavior of other formats.

## Limitations
This skill organizes supplied material and does not independently authenticate sources.
Absence of evidence does not prove a claim false.

## Troubleshooting
If evidence conflicts, record both observations and explain the unresolved difference.
If a claim is too broad to validate, request a narrower, measurable statement.
