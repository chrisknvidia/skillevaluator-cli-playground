# SkillEvaluator evaluation report

**Tier 1 scan result: FAILED**

1 skills · 0 passed · 1 failed · 0 incomplete

Errors: 3 · Warnings: 40

## Evaluation scope

Tier 1: executed for 1/1 skills with validator evidence; result FAILED\. Tier 2: Not run\. Tier 3: Not run\.

Recorded LLM stages: skipped\. LLM checks disabled by \-\-no\-llm\.

Static scanner outcomes do not establish behavioral usefulness. Not run tiers are not passes.

[Open full report](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559499179/1/index.html) · [Workflow run and logs](https://github.com/chrisknvidia/skillevaluator-cli-playground/actions/runs/41559499179)

**CI run conclusion:** failure

**Commit:** 184b994e2787f2d0e78cc11b270c9143b80de87a

**Runtime image:** ghcr\.io/nvidia/skillevaluator\-tier1@​sha256:c75c826f0e52d6c9a8d303ad7eefd606ed86e6940123f42b4eda2457863bcee7

## Needs attention

**skills/pdf / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/pdf/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/pdf / Security Scan (INCOMPLETE):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

Location: SKILL\.md:1

Suggested fix: Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**skills/pdf / License Compliance (FAIL):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

Location: LICENSE\.txt

Suggested fix: This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

## Skills and scores

| Skill | Tier 1 | Quality / 100 | Grade | Errors | Warnings |
| --- | --- | --- | --- | --- | --- |
| skills/pdf | FAIL | 74 | C | 3 | 40 |

## skills/pdf

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559499179/1/index.html#skill-001) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559499179/1/skill-001/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559499179/1/skill-001/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 65 | 0\.35 | 5 |
| discoverability | 75 | 0\.25 | 4 |
| reliability | 70 | 0\.25 | 5 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 8 | 1 | 6 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 1 | 2 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | FAIL | 0 | 1 | 0 |
| Code Risk Analysis | PASS | 2 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 14 |
| SCRIPT\_LINT | PASS | 0 | 0 | 17 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/pdf/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'pdf'

**Evidence metadata:** \{"description\_length": 437\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/pdf/

**Evidence: naming\_convention:** Folder name 'pdf' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 3\}

**Evidence: line\_count:** SKILL\.md within line limit \(314/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 314\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: optional\_files:** Found optional supporting files: scripts

**Evidence metadata:** \{"files\_found": \["scripts"\]\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'pdf'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'reference\.md' in skill root

**File:** /workspace/skills/pdf/reference\.md

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'forms\.md' in skill root

**File:** /workspace/skills/pdf/forms\.md

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/pdf/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/pdf/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'reference\.md' in skill root in /workspace/skills/pdf/reference\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'forms\.md' in skill root in /workspace/skills/pdf/forms\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/pdf/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'pdf'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/pdf/

**Scanner message:** \[OK\] naming\_convention: Folder name 'pdf' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(314/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] optional\_files: Found optional supporting files: scripts

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'pdf'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Unknown \(LP3\) \(medium\):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Keyword Baiting Trigger \(TR3\) \(medium\):** Trigger Abuse: Keyword Baiting Trigger: description clause 'Use this skill whenever the user wants to do anything with PDF files' is de

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Keyword Baiting Trigger: description clause 'Use this skill whenever the user wants to do anything with PDF files' is designed to match all or most user inputs Use descriptive triggers that clearly indicate the skill's purpose rather than generic keywords designed to maximize activation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Warning:** \[SECURITY\-MEDIUM\] MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\. in SKILL\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Trigger Abuse: Keyword Baiting Trigger: description clause 'Use this skill whenever the user wants to do anything with PDF files' is de in SKILL\.md:1

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 12 files for PII

**Evidence metadata:** \{"file\_count": 12\}

**Evidence: pii\_detection:** No PII detected in 12 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 12\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 12 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 12 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Finding: blocked\_license \(critical\):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

**File:** LICENSE\.txt

**Suggested fix:** This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

**Error:** \[LICENSE\-CRITICAL\] License 'Proprietary' is not allowed \(restrictive/copyleft\) in LICENSE\.txt

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Proprietary\. LICENSE\.txt has complete terms'

### Code Risk Analysis — evidence

**Evidence: bandit:** Bandit: No security issues found

**Evidence: semgrep:** Semgrep: No security issues found

**Scanner message:** Found 8 Python, 0 Shell, 0 JavaScript/TypeScript files

**Scanner message:** \[OK\] bandit: Bandit: No security issues found

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 3 markdown files for dead links

**Evidence metadata:** \{"file\_count": 3\}

**Evidence: dead\_links:** All relative links valid in 3 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 3\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 3 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 3 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 12 file\(s\)

**Evidence metadata:** \{"files\_scanned": 12\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 12 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 74\.0/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 74\.0, "skill\_type": "script\-based"\}

**Finding: quality\_correctness \(medium\):** No documented scripts in table format

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add '\#\# Available Scripts' with table: \| Script \| Purpose \| Arguments \|

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** Instructions don't mention 'run\_script'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add explicit run\_script\(\) call examples

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(437 chars, recommend 50\-150\)

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** Broad description without negative triggers may cause over\-triggering

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add boundary phrases like 'Do NOT use for\.\.\.'

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Skill name very short: 'pdf'

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Use descriptive names like 'crypto\-utils' not 'crypto'

**Finding metadata:** \{"deduction": 10, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No mention of error handling or validation

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Document expected errors and how to handle them

**Finding metadata:** \{"deduction": 10, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** Scripts may lack error handling: check\_fillable\_fields\.py, convert\_pdf\_to\_images\.py, create\_validation\_image\.py

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Scripts should handle errors explicitly

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/pdf/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-MEDIUM\] No documented scripts in table format in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Instructions don't mention 'run\_script' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(437 chars, recommend 50\-150\) in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Broad description without negative triggers may cause over\-triggering in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Skill name very short: 'pdf' in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No mention of error handling or validation in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Scripts may lack error handling: check\_fillable\_fields\.py, convert\_pdf\_to\_images\.py, create\_validation\_image\.py in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/pdf/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/pdf/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 74\.0/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Finding: magic\_numbers \(low\):** check\_bounding\_boxes\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/check\_bounding\_boxes\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** check\_bounding\_boxes\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/check\_bounding\_boxes\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: flat\_script \(medium\):** check\_fillable\_fields\.py has no function definitions \(flat script\)

**File:** /workspace/skills/pdf/scripts/check\_fillable\_fields\.py

**Suggested fix:** Wrap logic in functions for maintainability and testability

**Finding: missing\_shebang \(low\):** check\_fillable\_fields\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/check\_fillable\_fields\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: no\_input\_validation \(low\):** check\_fillable\_fields\.py may lack input validation

**File:** /workspace/skills/pdf/scripts/check\_fillable\_fields\.py

**Suggested fix:** Add argument checks and raise descriptive errors

**Finding: magic\_numbers \(low\):** convert\_pdf\_to\_images\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/convert\_pdf\_to\_images\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** convert\_pdf\_to\_images\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/convert\_pdf\_to\_images\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** create\_validation\_image\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/create\_validation\_image\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** create\_validation\_image\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/create\_validation\_image\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** extract\_form\_field\_info\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/extract\_form\_field\_info\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** extract\_form\_field\_info\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/extract\_form\_field\_info\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** extract\_form\_structure\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/extract\_form\_structure\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** extract\_form\_structure\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/extract\_form\_structure\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** fill\_fillable\_fields\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/fill\_fillable\_fields\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** fill\_fillable\_fields\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/fill\_fillable\_fields\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** fill\_pdf\_form\_with\_annotations\.py contains magic numbers

**File:** /workspace/skills/pdf/scripts/fill\_pdf\_form\_with\_annotations\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** fill\_pdf\_form\_with\_annotations\.py missing shebang line

**File:** /workspace/skills/pdf/scripts/fill\_pdf\_form\_with\_annotations\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Warning:** \[SCRIPT\_LINT\-LOW\] check\_bounding\_boxes\.py contains magic numbers in /workspace/skills/pdf/scripts/check\_bounding\_boxes\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] check\_bounding\_boxes\.py missing shebang line in /workspace/skills/pdf/scripts/check\_bounding\_boxes\.py

**Warning:** \[SCRIPT\_LINT\-MEDIUM\] check\_fillable\_fields\.py has no function definitions \(flat script\) in /workspace/skills/pdf/scripts/check\_fillable\_fields\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] check\_fillable\_fields\.py missing shebang line in /workspace/skills/pdf/scripts/check\_fillable\_fields\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] check\_fillable\_fields\.py may lack input validation in /workspace/skills/pdf/scripts/check\_fillable\_fields\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] convert\_pdf\_to\_images\.py contains magic numbers in /workspace/skills/pdf/scripts/convert\_pdf\_to\_images\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] convert\_pdf\_to\_images\.py missing shebang line in /workspace/skills/pdf/scripts/convert\_pdf\_to\_images\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] create\_validation\_image\.py contains magic numbers in /workspace/skills/pdf/scripts/create\_validation\_image\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] create\_validation\_image\.py missing shebang line in /workspace/skills/pdf/scripts/create\_validation\_image\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] extract\_form\_field\_info\.py contains magic numbers in /workspace/skills/pdf/scripts/extract\_form\_field\_info\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] extract\_form\_field\_info\.py missing shebang line in /workspace/skills/pdf/scripts/extract\_form\_field\_info\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] extract\_form\_structure\.py contains magic numbers in /workspace/skills/pdf/scripts/extract\_form\_structure\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] extract\_form\_structure\.py missing shebang line in /workspace/skills/pdf/scripts/extract\_form\_structure\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] fill\_fillable\_fields\.py contains magic numbers in /workspace/skills/pdf/scripts/fill\_fillable\_fields\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] fill\_fillable\_fields\.py missing shebang line in /workspace/skills/pdf/scripts/fill\_fillable\_fields\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] fill\_pdf\_form\_with\_annotations\.py contains magic numbers in /workspace/skills/pdf/scripts/fill\_pdf\_form\_with\_annotations\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] fill\_pdf\_form\_with\_annotations\.py missing shebang line in /workspace/skills/pdf/scripts/fill\_pdf\_form\_with\_annotations\.py

[Open full report](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559499179/1/index.html) · [Workflow run and logs](https://github.com/chrisknvidia/skillevaluator-cli-playground/actions/runs/41559499179)
