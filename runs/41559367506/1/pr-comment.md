**Tier 1 scan result: FAILED**

21 skills · 2 passed · 19 failed · 0 incomplete

| Skill | Status | Quality / 100 |
| --- | --- | --- |
| sandbox\-skills/evidence\-table | PASS | 98.2 / A |
| sandbox\-skills/glossary\-builder | PASS | 98.2 / A |
| skills/academy\-guide | FAIL | 88 / B |
| skills/algorithmic\-art | FAIL | 86 / B |
| skills/brand\-guidelines | FAIL | 84.2 / B |

16 more skills are listed in the full report.

## What to fix

First issue per affected skill; the full report contains all findings.

**skills/academy\-guide**

Problem: Security Scan: skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

Suggested fix: Check this validator's diagnostics and rerun after restoring the missing scan\.

**skills/algorithmic\-art**

Problem: Security Scan: skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

Suggested fix: Check this validator's diagnostics and rerun after restoring the missing scan\.

**skills/brand\-guidelines**

Problem: Author not specified in metadata

File: skills/brand\-guidelines/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/canvas\-design**

Problem: Security Scan: skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

Suggested fix: Check this validator's diagnostics and rerun after restoring the missing scan\.

**skills/claude\-api**

Problem: Security Scan: skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

Suggested fix: Check this validator's diagnostics and rerun after restoring the missing scan\.

**14 more affected skills:** open the full report.

Push your fixes to rerun PR checks, or rerun the workflow after resolving scan errors.

**CI run conclusion:** failure

Tier 1 static checks.

[Open full report](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html) · [Workflow run and logs](https://github.com/chrisknvidia/skillevaluator-cli-playground/actions/runs/41559367506)
