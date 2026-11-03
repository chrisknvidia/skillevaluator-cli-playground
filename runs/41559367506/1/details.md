# SkillEvaluator evaluation report

**Tier 1 scan result: FAILED**

21 skills · 2 passed · 19 failed · 0 incomplete

Errors: 151 · Warnings: 594

## Evaluation scope

Tier 1: executed for 21/21 skills with validator evidence; result FAILED\. Tier 2: Not run\. Tier 3: Not run\.

Recorded LLM stages: skipped\. LLM checks disabled by \-\-no\-llm\.

Static scanner outcomes do not establish behavioral usefulness. Not run tiers are not passes.

[Open full report](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html) · [Workflow run and logs](https://github.com/chrisknvidia/skillevaluator-cli-playground/actions/runs/41559367506)

**CI run conclusion:** failure

**Commit:** 87fd396eb165df31f9a120ac290af7affa50a278

**Runtime image:** ghcr\.io/nvidia/skillevaluator\-tier1@​sha256:c75c826f0e52d6c9a8d303ad7eefd606ed86e6940123f42b4eda2457863bcee7

## Needs attention

**skills/academy\-guide / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/academy\-guide/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/academy\-guide / Security Scan (INCOMPLETE):** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**skills/academy\-guide / Code Integrity &amp; Hygiene (FAIL):** Dead link in SKILL\.md: URL

**skills/algorithmic\-art / Schema &amp; Repository Governance (FAIL):** Missing top\-level heading \(\# Title\) in SKILL\.md body

Location: /workspace/skills/algorithmic\-art/SKILL\.md

Suggested fix: Add a top\-level heading after the frontmatter, e\.g\. '\# My Skill'

**skills/algorithmic\-art / Security Scan (INCOMPLETE):** analysis\-evasion: templates/generator\_template\.js \(partial\)

Location: SKILL\.md:396

Suggested fix: Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**skills/brand\-guidelines / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/brand\-guidelines/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/canvas\-design / Schema &amp; Repository Governance (FAIL):** Missing top\-level heading \(\# Title\) in SKILL\.md body

Location: /workspace/skills/canvas\-design/SKILL\.md

Suggested fix: Add a top\-level heading after the frontmatter, e\.g\. '\# My Skill'

**skills/canvas\-design / Security Scan (INCOMPLETE):** Excessive Agency: NOT LIMITED TO

Location: canvas\-fonts/ArsenalSC\-OFL\.txt:86

Suggested fix: Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**skills/claude\-api / Schema &amp; Repository Governance (FAIL):** Field 'name': Value error, Skill name 'claude\-api' must not contain reserved words \{'anthropic', 'claude'\}

Location: /workspace/skills/claude\-api/SKILL\.md

Suggested fix: Fix the 'name' field in frontmatter according to schema requirements

**skills/claude\-api / Security Scan (INCOMPLETE):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

Location: SKILL\.md:35

Suggested fix: Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**skills/claude\-api / PII Scan (FAIL):** Non\-placeholder email address: jane@​co\.com — 2 occurrences \(python/claude\-api/tool\-use\.md line 537; typescript/claude\-api/tool\-use\.md line 599\)

Location: python/claude\-api/tool\-use\.md:537

Suggested fix: Remove the address or use a placeholder like user@​example\.com

**skills/claude\-api / Code Risk Analysis (FAIL):** Audit url open for permitted schemes\. Allowing use of file:/ or custom schemes is often unexpected\. \(CWE\-22\)

Location: /workspace/skills/claude\-api/shared/preserved\-thinking\-migration/drop\_block\_probe\.py:435

Suggested fix: Review blacklist \(B310\) \(CWE\-22\)

**skills/claude\-api / QUALITY (FAIL):** Name contains reserved word \(anthropic, claude\)

Location: /workspace/skills/claude\-api/SKILL\.md

Suggested fix: Remove reserved words from skill name

**skills/discernment\-nudge / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/discernment\-nudge/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/discernment\-nudge / Security Scan (FAIL):** Anti\-Refusal: Always answer

Location: SKILL\.md:191

Suggested fix: Skill instructs the agent to never refuse or to always comply\. Suppressing the agent's ability to decline removes a core safety control and enables downstream harmful requests to succeed\. Remove any instruction telling the agent to never refuse or always comply\. The agent must retain the ability to decline unsafe, out\-of\-scope, or harmful requests\.

**skills/doc\-coauthoring / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/doc\-coauthoring/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/doc\-coauthoring / Security Scan (INCOMPLETE):** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**skills/docx / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/docx/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/docx / Security Scan (INCOMPLETE):** Tool Misuse: rm \-f \.\./out\.docx

Location: SKILL\.md:56

Suggested fix: Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**skills/docx / License Compliance (FAIL):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

Location: LICENSE\.txt

Suggested fix: This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

**skills/docx / Code Risk Analysis (FAIL):** Probable insecure usage of temp file/directory\. \(CWE\-377\)

Location: /workspace/skills/docx/scripts/accept\_changes\.py:16

Suggested fix: Review hardcoded\_tmp\_directory \(B108\) \(CWE\-377\)

**skills/frontend\-design / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/frontend\-design/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/frontend\-design / Security Scan (FAIL):** Anti\-Refusal: don't apologize

Location: SKILL\.md:69

Suggested fix: Skill instructs the agent to omit warnings, disclaimers, or ethical commentary\. Stripping safety caveats hides risk from the user and is a common jailbreak preamble\. Remove instructions that suppress warnings, disclaimers, or ethical commentary\. Let the agent surface safety\-relevant caveats to the user\.

**skills/internal\-comms / Schema &amp; Repository Governance (FAIL):** Missing top\-level heading \(\# Title\) in SKILL\.md body

Location: /workspace/skills/internal\-comms/SKILL\.md

Suggested fix: Add a top\-level heading after the frontmatter, e\.g\. '\# My Skill'

**skills/mcp\-builder / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/mcp\-builder/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/mcp\-builder / Security Scan (INCOMPLETE):** analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\)

Location: SKILL\.md:71

Suggested fix: Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**skills/mcp\-builder / PII Scan (FAIL):** Non\-placeholder email address: john@​acme\.com

Location: reference/node\_mcp\_server\_v2\.md:397

Suggested fix: Remove the address or use a placeholder like user@​example\.com

**skills/mcp\-builder / Code Risk Analysis (FAIL):** Using xml\.etree\.ElementTree\.parse to parse untrusted XML data is known to be vulnerable to XML attacks\. Replace xml\.etree\.ElementTree\.parse with its defusedxml equivalent function or make sure defusedxml\.defuse\_stdlib\(\) is called \(CWE\-20\)

Location: /workspace/skills/mcp\-builder/scripts/evaluation\.py:59

Suggested fix: Review blacklist \(B314\) \(CWE\-20\)

**skills/pdf / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/pdf/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/pdf / Security Scan (INCOMPLETE):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

Location: SKILL\.md:1

Suggested fix: Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**skills/pdf / License Compliance (FAIL):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

Location: LICENSE\.txt

Suggested fix: This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

**skills/pptx / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/pptx/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/pptx / Security Scan (INCOMPLETE):** Tool Misuse: rm \-f \.\./out\.pptx

Location: SKILL\.md:62

Suggested fix: Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**skills/pptx / License Compliance (FAIL):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

Location: LICENSE\.txt

Suggested fix: This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

**skills/skill\-creator / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/skill\-creator/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/skill\-creator / Security Scan (INCOMPLETE):** analysis\-evasion: assets/eval\_review\.html \(partial\)

Location: SKILL\.md:364

Suggested fix: Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**skills/slack\-gif\-creator / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/slack\-gif\-creator/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/slack\-gif\-creator / Security Scan (INCOMPLETE):** Supply Chain: pillow&gt;=10\.0\.0

Location: requirements\.txt:1

Suggested fix: Dependencies lack version pinning, allowing potential malicious package updates\. Consider pinning versions\. Pin all dependency versions in requirements\.txt or pyproject\.toml\. Use exact versions \(==\) or compatible ranges\. Run pip\-audit regularly\.

**skills/slack\-gif\-creator / Dependency Vulnerability Audit (INCOMPLETE):** Execution evidence is incomplete; inspect the validator details\.

**skills/theme\-factory / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/theme\-factory/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/theme\-factory / Security Scan (INCOMPLETE):** analysis\-evasion: theme\-showcase\.pdf \(partial\)

Location: SKILL\.md:23

Suggested fix: Referenced artifact was not completely inspected Provide inspectable source or analysis support for the referenced format\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**skills/web\-artifacts\-builder / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/web\-artifacts\-builder/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/web\-artifacts\-builder / Security Scan (INCOMPLETE):** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**skills/webapp\-testing / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/webapp\-testing/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/webapp\-testing / Security Scan (FAIL):** Tool Misuse: subprocess\.Popen\(                 server\['cmd'\],                 shell=True

Location: scripts/with\_server\.py:69

Suggested fix: Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**skills/webapp\-testing / Code Risk Analysis (FAIL):** Avoid subprocess calls with shell=True; pass an argument list without a shell\.

Location: /workspace/skills/webapp\-testing/scripts/with\_server\.py:69

Suggested fix: CWE: CWE\-78; OWASP: A03:2021 \- Injection

**skills/xlsx / Schema &amp; Repository Governance (FAIL):** Author not specified in metadata

Location: /workspace/skills/xlsx/SKILL\.md

Suggested fix: Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**skills/xlsx / Security Scan (INCOMPLETE):** Prompt Injection: ﻿

Location: scripts/office/schemas/ecma/fouth\-edition/opc\-contentTypes\.xsd:1

Suggested fix: Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**skills/xlsx / License Compliance (FAIL):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

Location: LICENSE\.txt

Suggested fix: This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

## Skills and scores

| Skill | Tier 1 | Quality / 100 | Grade | Errors | Warnings |
| --- | --- | --- | --- | --- | --- |
| sandbox\-skills/evidence\-table | PASS | 98.2 | A | 0 | 4 |
| sandbox\-skills/glossary\-builder | PASS | 98.2 | A | 0 | 4 |
| skills/academy\-guide | FAIL | 88 | B | 3 | 13 |
| skills/algorithmic\-art | FAIL | 86 | B | 4 | 17 |
| skills/brand\-guidelines | FAIL | 84.2 | B | 1 | 15 |
| skills/canvas\-design | FAIL | 79.2 | C | 3 | 45 |
| skills/claude\-api | FAIL | 79.8 | C | 73 | 108 |
| skills/discernment\-nudge | FAIL | 79.8 | C | 2 | 16 |
| skills/doc\-coauthoring | FAIL | 84.2 | B | 2 | 15 |
| skills/docx | FAIL | 74 | C | 10 | 47 |
| skills/frontend\-design | FAIL | 86.8 | B | 2 | 14 |
| skills/internal\-comms | FAIL | 79.2 | C | 2 | 18 |
| skills/mcp\-builder | FAIL | 81.5 | B | 13 | 36 |
| skills/pdf | FAIL | 74 | C | 3 | 40 |
| skills/pptx | FAIL | 77.8 | C | 9 | 45 |
| skills/skill\-creator | FAIL | 77.2 | C | 6 | 36 |
| skills/slack\-gif\-creator | FAIL | 88.5 | B | 2 | 25 |
| skills/theme\-factory | FAIL | 81.8 | B | 4 | 16 |
| skills/web\-artifacts\-builder | FAIL | 79 | C | 2 | 18 |
| skills/webapp\-testing | FAIL | 81.5 | B | 3 | 20 |
| skills/xlsx | FAIL | 71.5 | C | 7 | 42 |

## sandbox\-skills/evidence\-table

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-001) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-001/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-001/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 95 | 0\.35 | 1 |
| discoverability | 100 | 0\.25 | 0 |
| reliability | 100 | 0\.25 | 0 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | PASS | 10 | 0 | 2 |
| Semantic Version Validation | PASS | 1 | 0 | 0 |
| Security Scan | PASS | 1 | 0 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 1 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/sandbox\-skills/evidence\-table/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'evidence\-table'

**Evidence metadata:** \{"description\_length": 142\}

**Evidence: naming\_convention:** Folder name 'evidence\-table' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 14\}

**Evidence: line\_count:** SKILL\.md within line limit \(57/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 57\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: body\_recommended\_section:** Found recommended section: '\#\# Instructions' \(or '\#\# Usage'\)

**Evidence: body\_recommended\_section:** Found recommended section: '\#\# Examples'

**Evidence: optional\_files:** Skill directory contains only expected files

**Evidence: name\_consistency:** Directory name matches frontmatter: 'evidence\-table'

**Evidence: author\_format:** Valid author format: SkillEvaluator CI Demo Authors &lt;ci\-demo@​example\.com&gt;

**Finding: folder\_hierarchy \(medium\):** Skill not in standard location \(skills/ or team\-skills/\)

**File:** /workspace/sandbox\-skills/evidence\-table

**Suggested fix:** Move skill to skills/&lt;skill\-name&gt;/ or team\-skills/&lt;team&gt;/&lt;skill\-name&gt;/

**Warning:** \[SCHEMA\-MEDIUM\] Skill not in standard location \(skills/ or team\-skills/\) in /workspace/sandbox\-skills/evidence\-table

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'evidence\-table'

**Scanner message:** \[OK\] naming\_convention: Folder name 'evidence\-table' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(57/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] body\_recommended\_section: Found recommended section: '\#\# Instructions' \(or '\#\# Usage'\)

**Scanner message:** \[OK\] body\_recommended\_section: Found recommended section: '\#\# Examples'

**Scanner message:** \[OK\] optional\_files: Skill directory contains only expected files

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'evidence\-table'

**Scanner message:** \[OK\] author\_format: Valid author format: SkillEvaluator CI Demo Authors &lt;ci\-demo@​example\.com&gt;

### Semantic Version Validation — evidence

**Evidence: version\_semver:** Valid semantic version: 1\.0\.0

**Evidence metadata:** \{"previous\_version": null, "version": "1\.0\.0"\}

**Scanner message:** \[OK\] version\_semver: Valid semantic version: 1\.0\.0

### Security Scan — evidence

**Evidence: skillspector:** No security vulnerabilities detected \(secrets, API keys, credentials\)

**Scanner message:** \[OK\] skillspector: No security vulnerabilities detected \(secrets, API keys, credentials\)

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 1 files for PII

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: pii\_detection:** No PII detected in 1 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 1\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 1 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 1 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:** License: MIT \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 1 file\(s\)

**Evidence metadata:** \{"files\_scanned": 1\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 1 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 98\.2/100 \(Grade: A\)

**Evidence metadata:** \{"grade": "A", "overall\_score": 98\.2, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/sandbox\-skills/evidence\-table/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/sandbox\-skills/evidence\-table/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 98\.2/100 \(Grade: A\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## sandbox\-skills/glossary\-builder

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-002) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-002/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-002/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 95 | 0\.35 | 1 |
| discoverability | 100 | 0\.25 | 0 |
| reliability | 100 | 0\.25 | 0 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | PASS | 10 | 0 | 2 |
| Semantic Version Validation | PASS | 1 | 0 | 0 |
| Security Scan | PASS | 1 | 0 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 1 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/sandbox\-skills/glossary\-builder/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'glossary\-builder'

**Evidence metadata:** \{"description\_length": 133\}

**Evidence: naming\_convention:** Folder name 'glossary\-builder' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 16\}

**Evidence: line\_count:** SKILL\.md within line limit \(55/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 55\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: body\_recommended\_section:** Found recommended section: '\#\# Instructions' \(or '\#\# Usage'\)

**Evidence: body\_recommended\_section:** Found recommended section: '\#\# Examples'

**Evidence: optional\_files:** Skill directory contains only expected files

**Evidence: name\_consistency:** Directory name matches frontmatter: 'glossary\-builder'

**Evidence: author\_format:** Valid author format: SkillEvaluator CI Demo Authors &lt;ci\-demo@​example\.com&gt;

**Finding: folder\_hierarchy \(medium\):** Skill not in standard location \(skills/ or team\-skills/\)

**File:** /workspace/sandbox\-skills/glossary\-builder

**Suggested fix:** Move skill to skills/&lt;skill\-name&gt;/ or team\-skills/&lt;team&gt;/&lt;skill\-name&gt;/

**Warning:** \[SCHEMA\-MEDIUM\] Skill not in standard location \(skills/ or team\-skills/\) in /workspace/sandbox\-skills/glossary\-builder

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'glossary\-builder'

**Scanner message:** \[OK\] naming\_convention: Folder name 'glossary\-builder' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(55/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] body\_recommended\_section: Found recommended section: '\#\# Instructions' \(or '\#\# Usage'\)

**Scanner message:** \[OK\] body\_recommended\_section: Found recommended section: '\#\# Examples'

**Scanner message:** \[OK\] optional\_files: Skill directory contains only expected files

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'glossary\-builder'

**Scanner message:** \[OK\] author\_format: Valid author format: SkillEvaluator CI Demo Authors &lt;ci\-demo@​example\.com&gt;

### Semantic Version Validation — evidence

**Evidence: version\_semver:** Valid semantic version: 1\.0\.0

**Evidence metadata:** \{"previous\_version": null, "version": "1\.0\.0"\}

**Scanner message:** \[OK\] version\_semver: Valid semantic version: 1\.0\.0

### Security Scan — evidence

**Evidence: skillspector:** No security vulnerabilities detected \(secrets, API keys, credentials\)

**Scanner message:** \[OK\] skillspector: No security vulnerabilities detected \(secrets, API keys, credentials\)

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 1 files for PII

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: pii\_detection:** No PII detected in 1 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 1\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 1 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 1 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:** License: MIT \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 1 file\(s\)

**Evidence metadata:** \{"files\_scanned": 1\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 1 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 98\.2/100 \(Grade: A\)

**Evidence metadata:** \{"grade": "A", "overall\_score": 98\.2, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/sandbox\-skills/glossary\-builder/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/sandbox\-skills/glossary\-builder/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 98\.2/100 \(Grade: A\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/academy\-guide

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-003) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-003/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-003/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 80 | 0\.35 | 4 |
| discoverability | 95 | 0\.25 | 1 |
| reliability | 85 | 0\.25 | 3 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 7 | 1 | 4 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 1 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | FAIL | 3 | 1 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 8 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/academy\-guide/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'academy\-guide'

**Evidence metadata:** \{"description\_length": 992\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/academy\-guide/

**Evidence: naming\_convention:** Folder name 'academy\-guide' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 13\}

**Evidence: line\_count:** SKILL\.md within line limit \(147/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 147\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: name\_consistency:** Directory name matches frontmatter: 'academy\-guide'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/academy\-guide/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/academy\-guide/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'academy\-guide'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/academy\-guide/

**Scanner message:** \[OK\] naming\_convention: Folder name 'academy\-guide' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(147/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'academy\-guide'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 2 files for PII

**Evidence metadata:** \{"file\_count": 2\}

**Evidence: pii\_detection:** No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 2 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Error:** Dead link in SKILL\.md: URL

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 2 file\(s\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 2 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 88\.0/100 \(Grade: B\)

**Evidence metadata:** \{"grade": "B", "overall\_score": 88\.0, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(low\):** No examples provided

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add example usage with code blocks

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(992 chars, recommend 50\-150\)

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/academy\-guide/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-LOW\] No examples provided in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(992 chars, recommend 50\-150\) in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/academy\-guide/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/academy\-guide/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 88\.0/100 \(Grade: B\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/algorithmic\-art

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-004) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-004/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-004/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 85 | 0\.35 | 3 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 75 | 0\.25 | 4 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 6 | 2 | 5 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 2 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | PASS | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 0 | 0 | 2 |
| QUALITY | PASS | 1 | 0 | 9 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/algorithmic\-art/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'algorithmic\-art'

**Evidence metadata:** \{"description\_length": 324\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/algorithmic\-art/

**Evidence: naming\_convention:** Folder name 'algorithmic\-art' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 15\}

**Evidence: line\_count:** SKILL\.md within line limit \(405/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 405\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'algorithmic\-art'

**Finding: body\_heading \(high\):** Missing top\-level heading \(\# Title\) in SKILL\.md body

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add a top\-level heading after the frontmatter, e\.g\. '\# My Skill'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'templates' in skill root

**File:** /workspace/skills/algorithmic\-art/templates

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/algorithmic\-art/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Missing top\-level heading \(\# Title\) in SKILL\.md body in /workspace/skills/algorithmic\-art/SKILL\.md

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'templates' in skill root in /workspace/skills/algorithmic\-art/templates

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/algorithmic\-art/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'algorithmic\-art'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/algorithmic\-art/

**Scanner message:** \[OK\] naming\_convention: Folder name 'algorithmic\-art' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(405/500\)

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'algorithmic\-art'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: templates/generator\_template\.js \(partial\)

**File:** SKILL\.md

**Line:** 396

**Source line:** \- \*\*templates/generator\_template\.js\*\*: Reference for p5\.js best practices and code structure principles\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: templates/generator\_template\.js \(partial\) in SKILL\.md:396

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 2 files for PII

**Evidence metadata:** \{"file\_count": 2\}

**Evidence: pii\_detection:** No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 2 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: semgrep:** Semgrep: No security issues found

**Scanner message:** Found 0 Python, 0 Shell, 1 JavaScript/TypeScript files

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Finding: isolated\_invisible\_char \(low\):** Isolated invisible character\(s\) \(1\): VARIATION SELECTOR\-16

**File:** SKILL\.md

**Line:** 105

**Source line:** \#\#\# ⚠️ STEP 0: READ THE TEMPLATE FIRST ⚠️

**Suggested fix:** Likely a copy\-paste artifact\. Remove if not intentional\.

**Finding metadata:** \{"char\_count": 1, "unicode\_category": "variation\_selectors"\}

**Finding: isolated\_invisible\_char \(low\):** Isolated invisible character\(s\) \(1\): VARIATION SELECTOR\-16

**File:** SKILL\.md

**Line:** 105

**Source line:** \#\#\# ⚠️ STEP 0: READ THE TEMPLATE FIRST ⚠️

**Suggested fix:** Likely a copy\-paste artifact\. Remove if not intentional\.

**Finding metadata:** \{"char\_count": 1, "unicode\_category": "variation\_selectors"\}

**Warning:** \[UNICODE\-LOW\] Isolated invisible character\(s\) \(1\): VARIATION SELECTOR\-16 in SKILL\.md:105

**Warning:** \[UNICODE\-LOW\] Isolated invisible character\(s\) \(1\): VARIATION SELECTOR\-16 in SKILL\.md:105

### QUALITY — evidence

**Evidence: quality\_score:** Score: 86\.0/100 \(Grade: B\)

**Evidence metadata:** \{"grade": "B", "overall\_score": 86\.0, "skill\_type": "resource\-based"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(324 chars, recommend 50\-150\)

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No mention of error handling or validation

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Document expected errors and how to handle them

**Finding metadata:** \{"deduction": 10, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/algorithmic\-art/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(324 chars, recommend 50\-150\) in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No mention of error handling or validation in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/algorithmic\-art/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/algorithmic\-art/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 86\.0/100 \(Grade: B\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/brand\-guidelines

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-005) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-005/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-005/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 80 | 0\.35 | 4 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 75 | 0\.25 | 4 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 7 | 1 | 4 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | PASS | 1 | 0 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 10 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/brand\-guidelines/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'brand\-guidelines'

**Evidence metadata:** \{"description\_length": 236\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/brand\-guidelines/

**Evidence: naming\_convention:** Folder name 'brand\-guidelines' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 16\}

**Evidence: line\_count:** SKILL\.md within line limit \(73/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 73\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: name\_consistency:** Directory name matches frontmatter: 'brand\-guidelines'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/brand\-guidelines/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/brand\-guidelines/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'brand\-guidelines'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/brand\-guidelines/

**Scanner message:** \[OK\] naming\_convention: Folder name 'brand\-guidelines' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(73/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'brand\-guidelines'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Evidence: skillspector:** No security vulnerabilities detected \(secrets, API keys, credentials\)

**Scanner message:** \[OK\] skillspector: No security vulnerabilities detected \(secrets, API keys, credentials\)

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 2 files for PII

**Evidence metadata:** \{"file\_count": 2\}

**Evidence: pii\_detection:** No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 2 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 2 file\(s\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 2 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 84\.2/100 \(Grade: B\)

**Evidence metadata:** \{"grade": "B", "overall\_score": 84\.2, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(low\):** No examples provided

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add example usage with code blocks

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(236 chars, recommend 50\-150\)

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No mention of error handling or validation

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Document expected errors and how to handle them

**Finding metadata:** \{"deduction": 10, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/brand\-guidelines/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-LOW\] No examples provided in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(236 chars, recommend 50\-150\) in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No mention of error handling or validation in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/brand\-guidelines/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/brand\-guidelines/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 84\.2/100 \(Grade: B\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/canvas\-design

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-006) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-006/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-006/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 80 | 0\.35 | 4 |
| discoverability | 70 | 0\.25 | 4 |
| reliability | 75 | 0\.25 | 4 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 6 | 2 | 5 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 1 | 27 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 12 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/canvas\-design/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'canvas\-design'

**Evidence metadata:** \{"description\_length": 289\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/canvas\-design/

**Evidence: naming\_convention:** Folder name 'canvas\-design' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 13\}

**Evidence: line\_count:** SKILL\.md within line limit \(130/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 130\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'canvas\-design'

**Finding: body\_heading \(high\):** Missing top\-level heading \(\# Title\) in SKILL\.md body

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add a top\-level heading after the frontmatter, e\.g\. '\# My Skill'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'canvas\-fonts' in skill root

**File:** /workspace/skills/canvas\-design/canvas\-fonts

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/canvas\-design/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Missing top\-level heading \(\# Title\) in SKILL\.md body in /workspace/skills/canvas\-design/SKILL\.md

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'canvas\-fonts' in skill root in /workspace/skills/canvas\-design/canvas\-fonts

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/canvas\-design/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'canvas\-design'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/canvas\-design/

**Scanner message:** \[OK\] naming\_convention: Folder name 'canvas\-design' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(130/500\)

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'canvas\-design'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/ArsenalSC\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/BigShoulders\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Boldonse\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/BricolageGrotesque\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/CrimsonPro\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/DMMono\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/EricaOne\-OFL\.txt

**Line:** 87

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/GeistMono\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Gloock\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/IBMPlexMono\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/InstrumentSans\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Italiana\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/JetBrainsMono\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Jura\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/LibreBaskerville\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Lora\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/NationalPark\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/NothingYouCouldDo\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Outfit\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/PixelifySans\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/PoiretOne\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/RedHatMono\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Silkscreen\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/SmoochSans\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/Tektur\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/WorkSans\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Scope Creep \(EA3\) \(low\):** Excessive Agency: NOT LIMITED TO

**File:** canvas\-fonts/YoungSerif\-OFL\.txt

**Line:** 86

**Source line:**  DISCLAIMER THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AN

**Suggested fix:** Skill's behavior or capabilities extend beyond its stated purpose\. Scope creep allows an agent to perform actions unrelated to its documented functionality, increasing the attack surface\. Limit the skill's scope to its documented purpose\. Remove instructions that enable the agent to perform actions outside its stated functionality\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/ArsenalSC\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/BigShoulders\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Boldonse\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/BricolageGrotesque\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/CrimsonPro\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/DMMono\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/EricaOne\-OFL\.txt:87

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/GeistMono\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Gloock\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/IBMPlexMono\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/InstrumentSans\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Italiana\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/JetBrainsMono\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Jura\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/LibreBaskerville\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Lora\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/NationalPark\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/NothingYouCouldDo\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Outfit\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/PixelifySans\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/PoiretOne\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/RedHatMono\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Silkscreen\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/SmoochSans\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/Tektur\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/WorkSans\-OFL\.txt:86

**Warning:** \[SECURITY\-LOW\] Excessive Agency: NOT LIMITED TO in canvas\-fonts/YoungSerif\-OFL\.txt:86

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 29 files for PII

**Evidence metadata:** \{"file\_count": 29\}

**Evidence: pii\_detection:** No PII detected in 29 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 29\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 29 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 29 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 29 file\(s\)

**Evidence metadata:** \{"files\_scanned": 29\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 29 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 79\.2/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 79\.2, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(low\):** No examples provided

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add example usage with code blocks

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(289 chars, recommend 50\-150\)

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Description uses first/second person

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Use third person: 'Processes files' not 'I can process'

**Finding metadata:** \{"deduction": 15, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** Broad description without negative triggers may cause over\-triggering

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add boundary phrases like 'Do NOT use for\.\.\.'

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No mention of error handling or validation

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Document expected errors and how to handle them

**Finding metadata:** \{"deduction": 10, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/canvas\-design/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-LOW\] No examples provided in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(289 chars, recommend 50\-150\) in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Description uses first/second person in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Broad description without negative triggers may cause over\-triggering in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No mention of error handling or validation in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/canvas\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/canvas\-design/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 79\.2/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/claude\-api

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-007) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-007/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-007/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 70 | 0\.35 | 4 |
| discoverability | 85 | 0\.25 | 3 |
| reliability | 85 | 0\.25 | 3 |
| efficiency | 85 | 0\.15 | 1 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 1 | 2 | 1 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 67 | 96 |
| PII Scan | FAIL | 1 | 2 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | FAIL | 1 | 1 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | FAIL | 1 | 1 | 10 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/claude\-api/SKILL\.md"\}

**Finding: frontmatter\_field \(high\):** Field 'name': Value error, Skill name 'claude\-api' must not contain reserved words \{'anthropic', 'claude'\}

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Fix the 'name' field in frontmatter according to schema requirements

**Finding metadata:** \{"error\_type": "value\_error", "field": "name"\}

**Finding: frontmatter\_field \(high\):** Field 'description': String should have at most 1024 characters

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Fix the 'description' field in frontmatter according to schema requirements

**Finding metadata:** \{"error\_type": "string\_too\_long", "field": "description"\}

**Error:** \[SCHEMA\-HIGH\] Field 'name': Value error, Skill name 'claude\-api' must not contain reserved words \{'anthropic', 'claude'\} in /workspace/skills/claude\-api/SKILL\.md

**Error:** \[SCHEMA\-HIGH\] Field 'description': String should have at most 1024 characters in /workspace/skills/claude\-api/SKILL\.md

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 35

**Source line:** , and catch only the SDK's JSON error, never its typed API errors \- pattern in \`shared/tool\-use\-concepts\.md\` \-&gt; Eager input streaming\. Leave it off for non\-stre

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 128

**Source line:** ou approval gates, logging, error interception, and conditional execution \(see \`shared/tool\-use\-concepts\.md\`\) \- or the manual loop when you want to own the enti

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 464

**Source line:** vider availability varies by tool \- see \`shared/platform\-availability\.md\`\. See \`shared/tool\-use\-concepts\.md\` for \`pause\_turn\` handling\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 552

**Source line:** \-&gt; Read \`\{lang\}/claude\-api/README\.md\` \+ \`shared/tool\-use\-concepts\.md\` \(conceptual foundations: function calling, code execution, memory, structured outputs\) \+ \`

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 601

**Source line:** a named \`"bash"\` is a different tool\. Handler paths and security checks are in \`shared/tool\-use\-concepts\.md\` § Client\-Side Tools\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 602

**Source line:** ch advisors return plaintext vs encrypted \`advisor\_redacted\_result\` advice\) in \`shared/tool\-use\-concepts\.md\` § Advisor\. Availability: \`shared/platform\-availabil

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\)

**File:** SKILL\.md

**Line:** 606

**Source line:**  \`partial\_json\` may be incomplete \(\`max\_tokens\`\) or invalid \- guard the parse \(\`shared/tool\-use\-concepts\.md\` \-&gt; Eager input streaming\)\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 59

**Source line:** \| \`migrate\` \| Migrate existing Claude API code to a newer model\. \*\*Read \`shared/model\-migration\.md\` immediately\*\* and follow it in order: Step 0 \(confirm scope 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 64

**Source line:**  For the \*why\* \(the three\-step check, the append\-only edit table\) it chains to \`shared/model\-migration\.md\` \-&gt; Breaking change 3; do not summarize the guide \- ex

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 204

**Source line:** s also the default\), 128K max output\. Key API differences from Opus\-tier \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 for details:

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 207

**Source line:** unbilled \- nothing to strip; Claude Mythos 5\.1 instead reads them\); details in \`shared/model\-migration\.md\`\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 209

**Source line:** k model, so write the retry yourself and send it without \`between\_tools\` \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Sonnet 5\.5 \-&gt; Safeguards and f

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 212

**Source line:** ten for prior models are often too prescriptive and reduce output quality\. See \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 \-&gt; Behavioral shifts

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 213

**Source line:** horized by Anthropic\); no Priority Tier\. Same tokenizer as Claude Fable 5\. See \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 from Claude Fable 5\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 217

**Source line:** xtraction\`\. Fast mode is Claude API only, $8 / $40 per MTok \(2x standard\)\. See \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Opus 5\.5\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 221

**Source line:** : \`cyber\`, \`bio\`, \`frontier\_llm\`, \`reasoning\_extraction\`, \`general\_harms\`\. See \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Sonnet 5\.5\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 225

**Source line:**  break \(thinking table below\), and refusals have no server\-side fallback \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Haiku 5\.5\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 255

**Source line:** o 400s on forced \`tool\_choice\` \`any\`/\`tool\`, and runs preserved thinking \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Opus 5\.5\) \| Runs \*\*adaptive\*\* 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 258

**Source line:** o 400s on forced \`tool\_choice\` \`any\`/\`tool\`, and runs preserved thinking \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Sonnet 5\.5\) \| Runs \*\*adaptive\*

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 264

**Source line:** Opus 4\.8 keeps 4\.7's request surface \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Opus 4\.8 \(and \-&gt; Migrating to Opus 4\.7 from 4\.6 or earlier\)\. With \`thinki

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 268

**Source line:** l's between\-tool\-call progress notes as short \`thinking\` block summaries \- see \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 from Claude Fable 5 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 269

**Source line:** isting code that needs a hard token ceiling before you've tuned \`effort\` \- see \`shared/model\-migration\.md\` \-&gt; Transitional escape hatch\. It is fully removed on 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 327

**Source line:** e streaming so the large \`max\_tokens\` doesn't hit HTTP timeouts \(full details: \`shared/model\-migration\.md\` \-&gt; Task Budgets\):

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 412

**Source line:** ithout the beta, a text block after the tool results, earlier copies kept\. See \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 from Claude Fable 5 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 523

**Source line:** \-&gt; Read \`shared/model\-migration\.md\`

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 535

**Source line:** \-&gt; Read \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Opus 5\.5; the preserved\-thinking mechanics it points at are under Migrating to Claude Fable 5\.1 from 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 537

**Source line:** \-&gt; Read \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Sonnet 5\.5

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 539

**Source line:** \-&gt; Read \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 \-&gt; Behavioral shifts \(prompt\-tunable\) \+ Long\-running agent recommendations

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 541

**Source line:** \-&gt; Read \`shared/model\-migration\.md\` \-&gt; Migrating to Claude Fable 5\.1 from Claude Fable 5 \-&gt; New API features \+ Behavioral shifts \(prompt\-tunable\); for the histo

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 591

**Source line:** py\`", "migrate everything under \`services/\`", "update \`a\.py\` and \`b\.py\`"\)\. See \`shared/model\-migration\.md\` Step 0\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/model\-migration\.md \(partial\)

**File:** SKILL\.md

**Line:** 593

**Source line:** ssing\. Do not include internal or system XML tags in your response\."\* Details: \`shared/model\-migration\.md\` \-&gt; Two failure modes when thinking is disabled\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/prompt\-audit\.md \(partial\)

**File:** SKILL\.md

**Line:** 59

**Source line:** d, audit the in\-scope prompt text, tool descriptions, and request code against \`shared/prompt\-audit\.md\` \- prompting written for the source model is part of ever

**Suggested fix:** Referenced artifact was not completely inspected Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/prompt\-audit\.md \(partial\)

**File:** SKILL\.md

**Line:** 60

**Source line:** instructions the repository has outgrown or that contradict each other\. \*\*Read \`shared/prompt\-audit\.md\` immediately\*\* and follow it in order: Step 0 \(establish 

**Suggested fix:** Referenced artifact was not completely inspected Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/prompt\-audit\.md \(partial\)

**File:** SKILL\.md

**Line:** 545

**Source line:** \-&gt; Read \`shared/prompt\-audit\.md\` \- dated\-pattern tables with greppable signals, the keep list \(what NOT to delete\), and the report \+ proposed\-diff output contra

**Suggested fix:** Referenced artifact was not completely inspected Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/models\.md \(partial\)

**File:** SKILL\.md

**Line:** 200

**Source line:** equests an older model not in the table \(e\.g\., "opus 4\.5", "sonnet 3\.7"\), read \`shared/models\.md\` for the exact ID \- do not construct one yourself\.

**Suggested fix:** Referenced artifact was not completely inspected Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/models\.md \(partial\)

**File:** SKILL\.md

**Line:** 229

**Source line:** y the Models API \(\`client\.models\.retrieve\(id\)\` / \`client\.models\.list\(\)\`\) \- see \`shared/models\.md\` for the field reference and capability\-filter examples\.

**Suggested fix:** Referenced artifact was not completely inspected Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/anthropic\-cli\.md \(partial\)

**File:** SKILL\.md

**Line:** 244

**Source line:** Full auth details \(named profiles, scopes, the API\-key\-shadows\-profile trap, refresh\-token expiry\): \`shared/anthropic\-cli\.md\`\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/anthropic\-cli\.md \(partial\)

**File:** SKILL\.md

**Line:** 434

**Source line:** n\-controlled files synced with \`ant apply\` \- this is the recommended flow \(see \`shared/anthropic\-cli\.md\`\): the CLI owns the control plane \(creating and updating

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/anthropic\-cli\.md \(partial\)

**File:** SKILL\.md

**Line:** 442

**Source line:** te\)\. For attaching a terminal to a live session \(\`ant beta:sessions connect\`\): \`shared/anthropic\-cli\.md\`\.

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/managed\-agents\-multiagent\.md \(partial\)

**File:** SKILL\.md

**Line:** 446

**Source line:** gs, then summarize"\) \*\*or one loop would fill its context with reading:\*\* read \`shared/managed\-agents\-multiagent\.md\` and recommend a multiagent session \- start 

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: shared/managed\-agents\-multiagent\.md \(partial\)

**File:** SKILL\.md

**Line:** 448

**Source line:** across many items: would a roster have to batch the whole job's pieces?\): read \`shared/managed\-agents\-multiagent\.md\` § Dynamic workflows\. Set \`multiagent: \{"typ

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Context Leakage \(E4\) \(high\):** Data Exfiltration: send the full conversation history

**File:** python/claude\-api/README\.md

**Line:** 334

**Source line:**  \#\# Multi\-Turn Conversations  The API is stateless \- send the full conversation history each time\.  \`\`\`python class ConversationManager:

**Suggested fix:** Code or instructions that leak agent conversation context to external services, potentially exposing sensitive user interactions\. Remove any code that sends prompts, responses, or session data externally\. Preserve user privacy; never exfiltrate conversation content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Context Leakage \(E4\) \(high\):** Data Exfiltration: send the full conversation history

**File:** typescript/claude\-api/README\.md

**Line:** 256

**Source line:**  \#\# Multi\-Turn Conversations  The API is stateless \- send the full conversation history each time\. Use \`Anthropic\.MessageParam\[\]\` to type the messages array:  \`\`\`typescript const messages: Anthropic\.M

**Suggested fix:** Code or instructions that leak agent conversation context to external services, potentially exposing sensitive user interactions\. Remove any code that sends prompts, responses, or session data externally\. Preserve user privacy; never exfiltrate conversation content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Anti\-Refusal Statement \(AR2\) \(high\):** Anti\-Refusal: no warning

**File:** python/claude\-api/tool\-use\.md

**Line:** 68

**Source line:** \*\*Caution \- the runner does not auto\-resume \`pause\_turn\` \(as of \`anthropic\` 0\.116\.0\)\.\*\* A long\-running server\-tool turn can stop with \`stop\_reason: "pause\_turn"\`\. The runner only continues after a cli

**Suggested fix:** Skill instructs the agent to omit warnings, disclaimers, or ethical commentary\. Stripping safety caveats hides risk from the user and is a common jailbreak preamble\. Remove instructions that suppress warnings, disclaimers, or ethical commentary\. Let the agent surface safety\-relevant caveats to the user\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Anti\-Refusal Statement \(AR2\) \(high\):** Anti\-Refusal: no warning

**File:** typescript/claude\-api/tool\-use\.md

**Line:** 69

**Source line:** \*\*Caution \- the runner does not auto\-resume \`pause\_turn\` \(as of \`@​anthropic\-ai/sdk\` 0\.110\.0\)\.\*\* A long\-running server\-tool turn can stop with \`stop\_reason: "pause\_turn"\`\. The runner only continues aft

**Suggested fix:** Skill instructs the agent to omit warnings, disclaimers, or ethical commentary\. Stripping safety caveats hides risk from the user and is a common jailbreak preamble\. Remove instructions that suppress warnings, disclaimers, or ethical commentary\. Let the agent surface safety\-relevant caveats to the user\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Chaining Abuse \(TM2\) \(high\):** Tool Misuse: \| sudo 

**File:** shared/anthropic\-cli\.md

**Line:** 25

**Source line:**  \# Linux / WSL \- pick the release from github\.com/anthropics/anthropic\-cli/releases curl \-fsSL "https://github\.com/anthropics/anthropic\-cli/releases/download/v$\{VERSION\}/ant\_$\{VERSION\}\_$\(uname \-s \| tr

**Suggested fix:** Tool calls are chained to bypass individual safety checks or escalate capabilities beyond what any single tool call would allow\. Limit tool chaining depth and validate the output of each tool before passing it to the next\. Require explicit user approval for multi\-step chains\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: access token

**File:** shared/anthropic\-cli\.md

**Line:** 57

**Source line:** To hand the active credential to a subprocess or raw\-HTTP script:  \`\`\`sh \# Bare access token \- for curl's Authorization header curl https://api\.anthropic\.com/v1/messages \\   \-H "Authorization: Bearer 

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: access token

**File:** shared/managed\-agents\-tools\.md

**Line:** 353

**Source line:**   "auth": \{     "type": "mcp\_oauth",     "mcp\_server\_url": "https://mcp\.notion\.com/mcp",     "access\_token": "&lt;current access token&gt;",     "expires\_at": "2026\-04\-02T14:00:00Z",     "refresh": \{       

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: access token

**File:** shared/managed\-agents\-tools\.md

**Line:** 373

**Source line:** \| \`"client\_secret\_basic"\` \| \`\{type: "client\_secret\_basic", client\_secret: "\.\.\."\}\` \| Confidential client, secret via HTTP Basic auth \| \| \`"client\_secret\_post"\` \| \`\{type: "client\_secret\_post", client\_se

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: \.env 

**File:** shared/anthropic\-cli\.md

**Line:** 65

**Source line:**   \-H "content\-type: application/json" \\   \-d '\{"model": "claude\-opus\-5\-5", "max\_tokens": 1024, "messages": \[\{"role": "user", "content": "Hello"\}\]\}'  \# \.env format \- sets ANTHROPIC\_AUTH\_TOKEN \(and ANTH

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: External Model or Provider Selection \(EA5\) \(high\):** Excessive Agency: ant messages create \-\-model claude\-opus\-5\-5 \-\-max\-tokens 1024 \-\-message '\{role: user, content: "Hello"\}'

**File:** shared/anthropic\-cli\.md

**Line:** 85

**Source line:**  \`\`\`sh ant models list ant messages create \-\-model claude\-opus\-5\-5 \-\-max\-tokens 1024 \-\-message '\{role: user, content: "Hello"\}' ant beta:agents retrieve \-\-agent\-id agent\_01\.\.\. ant beta:sessions:events

**Suggested fix:** Skill selects an external model or provider that may use a different account or billing plan than the operator expects\. Undisclosed model switches can cause unexpected cost or quota consumption\. Remove the model/provider override or disclose it prominently and require explicit operator approval before invoking an external coding CLI or billed model\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: External Model or Provider Selection \(EA5\) \(high\):** Excessive Agency: ant messages create \-\-model claude\-opus\-5\-5 \-\-max\-tokens 1024 \\

**File:** shared/anthropic\-cli\.md

**Line:** 154

**Source line:** \`\`\`sh ant beta:agents create \-\-name "Researcher" \-\-model '\{id: claude\-sonnet\-5\-5\}' \-\-system @​\./prompts/researcher\.txt  ant messages create \-\-model claude\-opus\-5\-5 \-\-max\-tokens 1024 \\   \-\-message '\{rol

**Suggested fix:** Skill selects an external model or provider that may use a different account or billing plan than the operator expects\. Undisclosed model switches can cause unexpected cost or quota consumption\. Remove the model/provider override or disclose it prominently and require explicit operator approval before invoking an external coding CLI or billed model\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: Context Leakage \(E4\) \(high\):** Data Exfiltration: Extract context

**File:** shared/live\-sources\.md

**Line:** 87

**Source line:** \| \-\-\- \| \-\-\- \| \-\-\- \| \| Structured Outputs \| \`https://platform\.claude\.com/docs/en/build\-with\-claude/structured\-outputs\.md\` \| "Extract output\_config\.format usage and schema enforcement" \| \| Compaction \| 

**Suggested fix:** Code or instructions that leak agent conversation context to external services, potentially exposing sensitive user interactions\. Remove any code that sends prompts, responses, or session data externally\. Preserve user privacy; never exfiltrate conversation content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Context Leakage \(E4\) \(high\):** Data Exfiltration: Extract context

**File:** shared/live\-sources\.md

**Line:** 89

**Source line:** \| Compaction \| \`https://platform\.claude\.com/docs/en/build\-with\-claude/compaction\.md\` \| "Extract compaction setup, trigger config, and streaming with compaction" \| \| Context Editing \| \`https://platform

**Suggested fix:** Code or instructions that leak agent conversation context to external services, potentially exposing sensitive user interactions\. Remove any code that sends prompts, responses, or session data externally\. Preserve user privacy; never exfiltrate conversation content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: Access Token

**File:** shared/managed\-agents\-environments\.md

**Line:** 133

**Source line:** \|\-\-\-\|\-\-\-\|\-\-\-\| \| \`type\` \| Yes \| \`"github\_repository"\` \| \| \`url\` \| Yes \| The GitHub repository URL \| \| \`authorization\_token\` \| Yes \| GitHub Personal Access Token with repository access\. \*\*Never echoed i

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: External Script Fetching \(SC2\) \(high\):** Supply Chain: curl \| sh

**File:** shared/managed\-agents\-onboarding\-from\-url\.md

**Line:** 30

**Source line:** \- \*\*Pasted text or a local copy\*\* \(after a failed fetch\) keeps the tier of the URL in the request, never a higher one: first\-party only when the section says first\-party and the user confirms the text

**Suggested fix:** Remote code is downloaded and executed\. This bypasses code review and could introduce malicious code\. Avoid downloading and executing remote scripts\. Use trusted packages from PyPI/npm\. If remote fetch is required, verify checksums and use HTTPS\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: Chaining Abuse \(TM2\) \(high\):** Tool Misuse: &amp;&amp; sudo

**File:** shared/managed\-agents\-self\-hosted\-sandboxes\.md

**Line:** 187

**Source line:** \*\*Prepare the host\.\*\* POSIX \(Linux/macOS\) only; a case\-sensitive filesystem is recommended\. Before starting the worker:  \`\`\`bash sudo mkdir \-p /mnt/memory &amp;&amp; sudo chown "$USER" /mnt/memory \`\`\`  Do \*\*n

**Suggested fix:** Tool calls are chained to bypass individual safety checks or escalate capabilities beyond what any single tool call would allow\. Limit tool chaining depth and validate the output of each tool before passing it to the next\. Require explicit user approval for multi\-step chains\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Tool Parameter Abuse \(TM1\) \(high\):** Tool Misuse: rm \-rf /

**File:** shared/managed\-agents\-tools\.md

**Line:** 144

**Source line:**   "type": "agent\.tool\_use",   "id": "sevt\_01pqr\.\.\.",   "name": "bash",   "input": \{ "command": "rm \-rf /workspace/reports" \},   "evaluated\_permission": "deny",   "evaluation": \{     "type": "auto",

**Suggested fix:** Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: Tool Parameter Abuse \(TM1\) \(high\):** Tool Misuse: rm \-rf /workspace/reports

**File:** shared/managed\-agents\-tools\.md

**Line:** 144

**Source line:**   "type": "agent\.tool\_use",   "id": "sevt\_01pqr\.\.\.",   "name": "bash",   "input": \{ "command": "rm \-rf /workspace/reports" \},   "evaluated\_permission": "deny",   "evaluation": \{     "type": "auto",

**Suggested fix:** Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: Tool Parameter Abuse \(TM1\) \(high\):** Tool Misuse: rm \-rf /workspace/reports"

**File:** shared/managed\-agents\-tools\.md

**Line:** 144

**Source line:**   "type": "agent\.tool\_use",   "id": "sevt\_01pqr\.\.\.",   "name": "bash",   "input": \{ "command": "rm \-rf /workspace/reports" \},   "evaluated\_permission": "deny",   "evaluation": \{     "type": "auto",

**Suggested fix:** Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: Access Tokens

**File:** shared/managed\-agents\-tools\.md

**Line:** 336

**Source line:**  \*\*Do not put API keys in the system prompt or user messages as a workaround\*\* \- they persist in the session's event history\.  &gt; Formerly known internally as TATs \(Tool/Tenant Access Tokens\)\.  \*\*Flow:

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: YARA rule 'agent\_skill\_mcp\_tool\_poisoning\_metadata': MCP/tool metadata poisoning indicators in tool schemas or skill manifests \[agent\_skills\] \(YR4\) \(high\):** YARA Match: tools =; tools =; tools=; tools=; "tools":; tools":; "tools":; tools":; tools=; tools=; tools=; tools=; "tools":; tools":; tools:; tools:; tools:; parameters:; "description":; description":; "descript

**File:** shared/model\-migration\.md

**Line:** 406

**Source line:** laude\-opus\-4\-6",     thinking=\{"type": "adaptive"\},     output\_config=\{"effort": "high"\},     \.\.\. \) \`\`\`  \-\-\-  \#\# Additional Changes When Coming from 3\.x / 4\.0 / 4\.1 \-&gt; 4\.6  If you're jumping from Opus

**Suggested fix:** YARA rule matched a hack tool or exploit indicator \(offensive tools, reconnaissance, privilege escalation, or exploit frameworks\)\. Remove offensive tool references and exploit code\. Legitimate agent skills should not contain penetration testing tools, exploit frameworks, or reconnaissance utilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Context Leakage \(E4\) \(high\):** Data Exfiltration: send the conversation 

**File:** shared/model\-migration\.md

**Line:** 1446

**Source line:**  For languages not listed \(Java, Ruby, PHP\) \- or for a full runnable program in any language \- each public SDK repo ships a fallbacks example under \`examples/\` \(e\.g\. \`examples/fallbacks\.py\`, \`examples

**Suggested fix:** Code or instructions that leak agent conversation context to external services, potentially exposing sensitive user interactions\. Remove any code that sends prompts, responses, or session data externally\. Preserve user privacy; never exfiltrate conversation content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Memory Manipulation \(MP3\) \(high\):** Memory Poisoning: new name is

**File:** shared/preserved\-thinking\-migration/causes\.md

**Line:** 37

**Source line:** " error if the model still calls it \| \| 2 \| \`tool\_schema\_changed\` \(\`tools\_changed\`\) \| Same tool names, different description or schema text: a date, a refreshed token, a live listing, a version inside

**Suggested fix:** Skill manipulates agent memory, state, or stored context\. Memory corruption can alter personality, override safety rules, or cause unpredictable behavior\. Protect agent memory and state from modification by untrusted content\. Use read\-only memory for critical instructions and validate all state changes\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: MCP Config Access \(AS2\) \(high\):** Agent Snooping: mcp\.json\`\) can hold secret

**File:** shared/prompt\-audit\.md

**Line:** 33

**Source line:** vel outside dependency directories, with the instruction files they import \(an import that points at anything else is reported by path, not read\); rule files \(\`\.claude/rules/\`, \`\.cursorrules\`\-style\); 

**Suggested fix:** Skill accesses MCP server configuration files \(such as mcp\.json or claude\_desktop\_config\.json\)\. MCP configs contain server URLs, authentication tokens, and tool definitions — reading them allows the skill to discover and potentially abuse other tool integrations\. Remove all code or instructions that read MCP configuration files \(such as mcp\.json or claude\_desktop\_config\.json\)\. MCP server details should be managed by the agent runtime, not read by individual skills\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: External Model or Provider Selection \(EA5\) \(high\):** Excessive Agency: ant messages count\-tokens \-\-model claude\-opus\-5\-5 \\

**File:** shared/token\-counting\.md

**Line:** 31

**Source line:** \#\# CLI  \`\`\`sh ant messages count\-tokens \-\-model claude\-opus\-5\-5 \\   \-\-message '\{role: user, content: "@​\./CLAUDE\.md"\}' \\   \-\-transform input\_tokens \-r \`\`\`

**Suggested fix:** Skill selects an external model or provider that may use a different account or billing plan than the operator expects\. Undisclosed model switches can cause unexpected cost or quota consumption\. Remove the model/provider override or disclose it prominently and require explicit operator approval before invoking an external coding CLI or billed model\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: Unknown \(LP3\) \(medium\):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** SKILL\.md

**Line:** 71

**Source line:**  \#\# Language Detection  Before reading code examples, determine which language the user is working in \(exception: for the \`prompt\-audit\` subcommand, skip this section's ask steps \- the audit is non\-in

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** SKILL\.md

**Line:** 591

**Source line:** diting:\*\* When a user asks to migrate code to a newer Claude model without naming a specific file, directory, or file list, \*\*ask which scope to apply first\*\* \- the entire working directory, a specifi

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-onboarding\-from\-quickstart\.md

**Line:** 54

**Source line:** \| Question \| When \| Options \| \|\-\-\-\|\-\-\-\|\-\-\-\| \| \*\*Use this template?\*\* \| always \| \`Use this template\` / \`Cancel\` \| \| \*\*Should it confirm before acting?\*\* \| \`agent\.md\` has \`mcp\_servers\` \| \`Run without as

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-onboarding\-from\-quickstart\.md

**Line:** 57

**Source line:** mpted, which is what the Console sets / \`Judge risky actions\` \- writes, posts and changes are judged call by call, and a run can pause for you \| \| \*\*Credentials as listed?\*\* \| \`agent\.md\` has \`mcp\_serv

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-onboarding\-from\-quickstart\.md

**Line:** 58

**Source line:** ing\` \|     \- \*\*Recommend \`Judge risky actions\` when the file has a deployment section\*\* \(nobody is watching a scheduled run\) \*\*or the prompt reads text that outsiders write\*\* \(web pages, customer mess

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-quickstarts/bug\-hunter\.md

**Line:** 74

**Source line:** \- Each agent works only in its own folder under /tmp/hunt, which you name in its brief, and never opens another agent's folder\. \- Agents install and download nothing\. Any network access is only for ge

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-quickstarts/explainer\-video\-maker\.md

**Line:** 70

**Source line:** \- Leave tools out of define as well, always\. A run's agents get their tools from the engine, which hands down yours and nothing more\. \- One agent failing must not fail the run\. Ask agents for short an

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-quickstarts/performance\-tuner\.md

**Line:** 86

**Source line:** \- Leave tools out of define as well, always\. The agents in a run get their tools from the engine, which hands down yours and nothing more\. \- One agent failing must not fail the run\. A function whose o

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/managed\-agents\-quickstarts/watchlist\-scanner\.md

**Line:** 69

**Source line:** \- Give the run a 30\-minute time limit, or 60 minutes for a deep scan\. \- One agent failing must not fail the run\. A ticker whose scan failed is listed as not covered, never as neutral\. \- Write the repo

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/model\-migration\.md

**Line:** 53

**Source line:** 2\. A specific subdirectory \(e\.g\. \`src/\`, \`app/\`, \`services/billing/\`\) 3\. A specific file or a list of files  Surface this as a single clarifying question so the user can answer in one turn\. \*\*Proceed 

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/model\-migration\.md

**Line:** 1502

**Source line:** p into long sessions it can occasionally end a turn with a text\-only statement of intent \("I'll now run X"\) without the tool call, or ask permission it doesn't need\. A "continue" recovers it interacti

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without asking

**File:** shared/model\-migration\.md

**Line:** 1813

**Source line:** n in § Migrating to Claude Fable 5\.1 above and the test\-coverage line below\. If your existing prompt asks the model to test or check its work before reporting, \*\*keep it\*\* when migrating \- the Claude 

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: write \`claude\-fable\-5\-1\`, \`claude\-opus\-5\-5\`, \`claude\-opus\-5\`, or \`claude\-sonnet\-5\-5\` code, include the server\-side \`fallbacks\` parameter by default\*\* \(for \`claude\-sonnet\-5\-5\`, only the \`"default"\` for

**File:** SKILL\.md

**Line:** 209

**Source line:**  with Opus 4\.7\)\. Token counts are roughly unchanged when migrating from Opus 4\.7/4\.8; per\-token pricing differs\. Coming from Opus 4\.6, Sonnet, Haiku, or older, re\-baseline with \`count\_tokens\` \(the Opu

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: don't ask the user

**File:** SKILL\.md

**Line:** 237

**Source line:**  mean there are no credentials\.\*\* The SDKs and the \`ant\` CLI resolve credentials in this order \(first match wins\): \`ANTHROPIC\_API\_KEY\` \-&gt; \`ANTHROPIC\_AUTH\_TOKEN\` \-&gt; the \`ANTHROPIC\_PROFILE\`\-selected or 

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Context Window Stuffing \(MP2\) \(medium\):** Memory Poisoning: exceed context window

**File:** SKILL\.md

**Line:** 520

**Source line:** \*\*Chat UI or real\-time response display:\*\* \-&gt; Read \`\{lang\}/claude\-api/README\.md\` \+ \`\{lang\}/claude\-api/streaming\.md\`  \*\*Long\-running conversations \(may exceed context window\):\*\* \-&gt; Read \`\{lang\}/claude\-

**Suggested fix:** Skill attempts to fill the context window with filler content, displacing legitimate instructions and safety constraints\. This can degrade agent performance or bypass safety boundaries\. Implement context\-window management that detects and rejects padding or stuffing attempts\. Prioritize system instructions over user\-injected content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: cURL / Raw HTTP  Use these examples when the user needs raw HTTP requests or is working in a language without an official SDK\.  \#\# Setup  \`\`\`bash export ANTHROPIC\_API\_KEY="your\-api\-key" \`\`\`  \-\-\-  \#\# B

**File:** curl/examples\.md

**Line:** 1

**Source line:** \# Claude API \- cURL / Raw HTTP  Use these examples when the user needs raw HTTP requests or is working in a language without an official SDK\. 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 16

**Source line:** \#\# Basic Message Request  \`\`\`bash curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 37

**Source line:**  \`\`\`bash \# Capture the response, then extract fields response=$\(curl \-s https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "ant

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 63

**Source line:** \#\# Streaming \(SSE\)  \`\`\`bash curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 102

**Source line:** \#\# Tool Use  \`\`\`bash curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 127

**Source line:** When Claude responds with a \`tool\_use\` block, send the result back:  \`\`\`bash curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 165

**Source line:** Put \`cache\_control\` on the last block of the stable prefix\. See \`shared/prompt\-caching\.md\` for placement patterns and the silent\-invalidator audit checklist\.  \`\`\`bash curl https://api\.anthropic\.com/v1

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 192

**Source line:**  \`\`\`bash \# Fable 5 / Claude Opus 5\.5 / Claude Opus 5 / Opus 4\.8 / 4\.7 / 4\.6: adaptive thinking \(recommended\) curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/examples\.md

**Line:** 217

**Source line:** On \`claude\-fable\-5\-1\`, safety classifiers may decline a request \(HTTP 200 with \`stop\_reason: "refusal"\`\)\. Fallbacks are \*\*opt\-in\*\*: without them the request simply stops\. Include the \`fallbacks\` param

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 24

**Source line:** \#\# Create an Environment  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/environments \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "name": "my\-dev\-env",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 38

**Source line:** \#\#\# Allowing specific hosts  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/environments \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "name": "restricted\-env",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 66

**Source line:**  \`\`\`bash \# 1\. Create the agent curl \-X POST https://api\.anthropic\.com/v1/agents \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "name": "Coding Assistant",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 85

**Source line:** \# \-&gt; \{ "id": "agent\_abc123", \.\.\. \}  \# 2\. Start a session curl \-X POST https://api\.anthropic\.com/v1/sessions \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "agent": \{ "type": "agent", "id": "agent\_abc123", "version

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 99

**Source line:**  \`\`\`bash \# 1\. Create the agent curl \-X POST https://api\.anthropic\.com/v1/agents \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "name": "Code Reviewer",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 130

**Source line:**   \}'  \# 2\. Start a session with the repo mounted curl \-X POST https://api\.anthropic\.com/v1/sessions \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "agent": \{ "type": "agent", "id": "agent\_abc123", "version": 1 \},

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 153

**Source line:** \`\`\`bash \# Create a session with a hard $25\.00 spend cap \(list\-priced; USD only; create\-only\)\. \# amount is in minor units \(cents\) as an integer string: "2500" = $25\.00 curl \-X POST https://api\.anthropi

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 166

**Source line:**  \# Change the cap \- higher or lower, but it must exceed the consumed list cost\. \# An accepted update resumes work paused at budget\_reached curl \-X POST https://api\.anthropic\.com/v1/sessions/$SESSION\_I

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 171

**Source line:**   \-d '\{ "budget": \{ "type": "limit", "max\_list\_cost": \{ "amount": "4000", "currency": "USD" \} \} \}'  \# Remove the cap entirely \- one\-way; a removed budget can never be re\-added curl \-X POST https://api

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 183

**Source line:** \#\# Send a User Message  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/sessions/$SESSION\_ID/events \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "events": \[

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 200

**Source line:** \#\# Stream Events \(SSE\)  \`\`\`bash curl \-N https://api\.anthropic\.com/v1/sessions/$SESSION\_ID/events/stream \\   "$\{HEADERS\[@​\]\}" \`\`\` 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 225

**Source line:**  \`\`\`bash \# Get all events curl https://api\.anthropic\.com/v1/sessions/$SESSION\_ID/events \\   "$\{HEADERS\[@​\]\}"  \# Paginated \- get next page of events

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 229

**Source line:**   "$\{HEADERS\[@​\]\}"  \# Paginated \- get next page of events curl "https://api\.anthropic\.com/v1/sessions/$SESSION\_ID/events?page=page\_abc123" \\   "$\{HEADERS\[@​\]\}" \`\`\` 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 240

**Source line:** When the agent calls a custom tool, send the result back:  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/sessions/$SESSION\_ID/events \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "events": \[

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 260

**Source line:** An \`agent\.tool\_use\` / \`agent\.mcp\_tool\_use\` event with \`"evaluated\_permission": "ask"\` \(\`always\_ask\`, or \`auto\` with no determination\) waits until you answer it\. Send that event's \`id\` as \`tool\_use\_id\`

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 278

**Source line:** \#\# Interrupt a Running Session  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/sessions/$SESSION\_ID/events \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "events": \[

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 294

**Source line:** \#\# Get Session Details  \`\`\`bash curl https://api\.anthropic\.com/v1/sessions/$SESSION\_ID \\   "$\{HEADERS\[@​\]\}" \`\`\` 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 303

**Source line:** \#\# List Sessions  \`\`\`bash curl https://api\.anthropic\.com/v1/sessions \\   "$\{HEADERS\[@​\]\}" \`\`\` 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 312

**Source line:** \#\# Delete a Session  \`\`\`bash curl \-X DELETE https://api\.anthropic\.com/v1/sessions/$SESSION\_ID \\   "$\{HEADERS\[@​\]\}" \`\`\` 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 321

**Source line:** \#\# Upload a File  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/files \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-F "file=@​path/to/file\.txt"

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 335

**Source line:**  \`\`\`bash \# List files associated with a session curl "https://api\.anthropic\.com/v1/files?scope\_id=%24SESSION\_ID" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-H "a

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 341

**Source line:**   \-H "anthropic\-beta: managed\-agents\-2026\-04\-01"  \# Download a specific file curl "https://api\.anthropic\.com/v1/files/$FILE\_ID/content" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 352

**Source line:** \#\# List Agents  \`\`\`bash curl https://api\.anthropic\.com/v1/agents \\   "$\{HEADERS\[@​\]\}" \`\`\` 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 362

**Source line:**  \`\`\`bash \# 1\. Agent declares MCP server \(no auth here \- auth goes in a vault\) curl \-X POST https://api\.anthropic\.com/v1/agents \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "name": "MCP Agent",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 384

**Source line:**   \}'  \# 2\. Session attaches vault containing credentials for that MCP server URL curl \-X POST https://api\.anthropic\.com/v1/sessions \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "agent": "agent\_abc123",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** curl/managed\-agents\.md

**Line:** 400

**Source line:** \#\# Tool Configuration  \`\`\`bash curl \-X POST https://api\.anthropic\.com/v1/agents \\   "$\{HEADERS\[@​\]\}" \\   \-d '\{     "name": "Restricted Agent",

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** php/managed\-agents/README\.md

**Line:** 248

**Source line:**  // Raw cURL upload \(canonical example from the apps source\) $csvPath = 'data\.csv'; $ch = curl\_init\('https://api\.anthropic\.com/v1/files'\); curl\_setopt\_array\($ch, \[     CURLOPT\_RETURNTRANSFER =&gt; true, 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** shared/admin\-api\.md

**Line:** 5

**Source line:**  Read this file when the user wants to manage their Anthropic organization programmatically: members and roles, invites, workspaces and workspace members, API keys, rate limit reports, service account

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** shared/anthropic\-cli\.md

**Line:** 58

**Source line:**  \`\`\`sh \# Bare access token \- for curl's Authorization header curl https://api\.anthropic\.com/v1/messages \\   \-H "Authorization: Bearer $\(ant auth print\-credentials \-\-access\-token\)" \\   \-H "anthropic\-ve

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** shared/managed\-agents\-scheduled\-deployments\.md

**Line:** 16

**Source line:** \- \`schedule\` takes a cron \`expression\` and an IANA \`timezone\`\. Minute\-level granularity is the maximum\.  \`\`\`bash curl \-fsSL https://api\.anthropic\.com/v1/deployments \\   \-H "x\-api\-key: $ANTHROPIC\_API\_K

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.anthropic\.com/

**File:** shared/models\.md

**Line:** 35

**Source line:** \#\#\# Raw HTTP  \`\`\`bash curl https://api\.anthropic\.com/v1/models/claude\-opus\-4\-8 \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \`\`\`

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-d '\{     "model": "claude\-opus\-5\-5

**File:** curl/examples\.md

**Line:** 63

**Source line:** \#\# Streaming \(SSE\)  \`\`\`bash curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: cURL / Raw HTTP  Use these examples when the user needs raw HTTP requests or is working without an SDK\.  \#\# Setup  \`\`\`bash export ANTHROPIC\_API\_KEY="your\-api\-key"  \# Common headers HEADERS=\(   \-H "Con

**File:** curl/managed\-agents\.md

**Line:** 1

**Source line:** \# Managed Agents \- cURL / Raw HTTP  Use these examples when the user needs raw HTTP requests or is working without an SDK\. 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: automatically run

**File:** go/claude\-api/tool\-use\.md

**Line:** 56

**Source line:**     log\.Fatal\(err\) \}  // Create a tool runner that handles the conversation loop automatically runner := client\.Beta\.Messages\.NewToolRunner\(     \[\]anthropic\.BetaTool\{weatherTool\},     anthropic\.BetaTo

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: automatically run

**File:** python/claude\-api/tool\-use\.md

**Line:** 42

**Source line:**     \# Your implementation here     return f"72°F and sunny in \{location\}"  \# The tool runner handles the agentic loop automatically runner = client\.beta\.messages\.tool\_runner\(     model="claude\-opus\-5\-

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** go/managed\-agents/README\.md

**Line:** 430

**Source line:**     MCPServers: \[\]anthropic\.BetaManagedAgentsURLMCPServerParams\{\{         Type: anthropic\.BetaManagedAgentsURLMCPServerParamsTypeURL,         Name: "github",         URL:  "https://api\.githubcopilot\.c

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** java/managed\-agents/README\.md

**Line:** 342

**Source line:**     \.addMcpServer\(BetaManagedAgentsUrlMcpServerParams\.builder\(\)         \.type\(BetaManagedAgentsUrlMcpServerParams\.Type\.URL\)         \.name\("github"\)         \.url\("https://api\.githubcopilot\.com/mcp/"\)  

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** php/managed\-agents/README\.md

**Line:** 353

**Source line:**         BetaManagedAgentsURLMCPServerParams::with\(             type: 'url',             name: 'github',             url: 'https://api\.githubcopilot\.com/mcp/',         \),     \],     tools: \[

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** ruby/managed\-agents/README\.md

**Line:** 297

**Source line:**     \{       type: "url",       name: "github",       url: "https://api\.githubcopilot\.com/mcp/"     \}   \],   tools: \[

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** shared/managed\-agents\-api\-reference\.md

**Line:** 259

**Source line:**     \{       "type": "url",       "name": "github",       "url": "https://api\.githubcopilot\.com/mcp/"     \}   \],   "multiagent": \{

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** shared/managed\-agents\-environments\.md

**Line:** 154

**Source line:**     name: 'GitHub Agent',     model: 'claude\-opus\-5\-5',     mcp\_servers: \[       \{ type: 'url', name: 'github', url: 'https://api\.githubcopilot\.com/mcp/' \},     \],     tools: \[       \{

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** shared/managed\-agents\-environments\.md

**Line:** 197

**Source line:**     mcp\_servers=\[\{         "type": "url",         "name": "github",         "url": "https://api\.githubcopilot\.com/mcp/",     \}\],     tools=\[         \{

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.githubcopilot\.com/

**File:** shared/managed\-agents\-quickstarts/incident\-commander\.md

**Line:** 31

**Source line:**     url: https://mcp\.slack\.com/mcp   \- name: github     type: url     url: https://api\.githubcopilot\.com/mcp/ tools:   \- type: agent\_toolset\_20260401   \- type: mcp\_toolset

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without checking

**File:** php/claude\-api/README\.md

**Line:** 69

**Source line:** \);  // content is an array of polymorphic blocks \(TextBlock, ToolUseBlock, // ThinkingBlock\)\. Accessing \-&gt;text on content\[0\] without checking the block // type will throw if the first block is not a T

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: without checking

**File:** shared/managed\-agents\-outcomes\.md

**Line:** 69

**Source line:** \| \`needs\_revision\` \| Agent starts another iteration\. \| \| \`max\_iterations\_reached\` \| No further grader cycles\. Agent may run one final revision, then session \-&gt; \`idle\`\. \| \| \`failed\` \| Session \-&gt; \`idle\`

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Unbounded Resource Access \(EA4\) \(medium\):** Excessive Agency: max\_retries=0

**File:** python/claude\-api/README\.md

**Line:** 57

**Source line:**  \#\#\# Retries  The SDK auto\-retries connection errors, 408, 409, 429, and &gt;=500 with exponential backoff \(default 2 retries\)\. Set \`max\_retries\` on the client or via \`with\_options\(\)\`; \`max\_retries=0\` di

**Suggested fix:** Skill allows unbounded resource consumption \(API calls, storage, compute\)\. Without rate limits or quotas, a compromised or misbehaving agent can cause denial\-of\-service or cost overruns\. Set explicit rate limits, timeouts, and resource quotas for API calls, file operations, and compute\. Implement circuit breakers for runaway loops\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Context Window Stuffing \(MP2\) \(medium\):** Memory Poisoning: exceed the context window

**File:** shared/agent\-design\.md

**Line:** 80

**Source line:** \| Pattern \| When to use it \| What to expect \| \| \-\-\- \| \-\-\- \| \-\-\- \| \| \*\*Context editing\*\* \| Context grows stale over many turns \(old tool results, completed thinking\)\. \| Tool results and thinking blocks

**Suggested fix:** Skill attempts to fill the context window with filler content, displacing legitimate instructions and safety constraints\. This can degrade agent performance or bypass safety boundaries\. Implement context\-window management that detects and rejects padding or stuffing attempts\. Prioritize system instructions over user\-injected content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Sudo/Root Execution \(PE2\) \(medium\):** Privilege Escalation: sudo 

**File:** shared/anthropic\-cli\.md

**Line:** 25

**Source line:**  \# Linux / WSL \- pick the release from github\.com/anthropics/anthropic\-cli/releases curl \-fsSL "https://github\.com/anthropics/anthropic\-cli/releases/download/v$\{VERSION\}/ant\_$\{VERSION\}\_$\(uname \-s \| tr

**Suggested fix:** Commands invoke sudo or root privileges\. Verify this elevated access is necessary and justified\. Avoid sudo/root unless strictly required\. Prefer least\-privilege patterns\. If elevation is needed, document the justification and scope\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: curl https://api\.anthropic\.com/v1/messages \\   \-H "Authorization: Bearer $\(ant auth print\-credentials \-\-access\-token\)" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-H "anthropic\-beta: oauth\-2025\-04\-20" 

**File:** shared/anthropic\-cli\.md

**Line:** 58

**Source line:**  \`\`\`sh \# Bare access token \- for curl's Authorization header curl https://api\.anthropic\.com/v1/messages \\   \-H "Authorization: Bearer $\(ant auth print\-credentials \-\-access\-token\)" \\   \-H "anthropic\-ve

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: skills/pr\-summary/SKILL\.md

**File:** shared/anthropic\-cli\.md

**Line:** 171

**Source line:** \`\`\` agents/summarizer\.md          \# YAML frontmatter = agent config, Markdown body = system prompt environments/cloud\.yaml       \# the environment create body skills/pr\-summary/SKILL\.md    \# a skill i

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: ls stored in its root \`\.claude/skills

**File:** shared/managed\-agents\-environments\.md

**Line:** 123

**Source line:**  Clones a GitHub repository into the session container during initialization, before the agent begins execution\. The agent can read, edit, commit, and push via \`bash\` \(\`git\`\)\. Multiple repositories pe

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: skills/brief\-format/SKILL\.md

**File:** shared/managed\-agents\-onboarding\-from\-url\.md

**Line:** 108

**Source line:**     vault\.yaml                \# type: vault \- the container only, never a secret\. No credentials \-&gt; no file     deployment\-daily\.yaml     \# one per schedule \(a \.md whose body is the kickoff message wo

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: ls from a GitHub repository\) \- root \`\.claude/skills

**File:** shared/managed\-agents\-overview\.md

**Line:** 64

**Source line:** /managed\-agents\-core\.md\` \(§ Session budgets\) \- \`budget\` at session create, \`budget\_reached\` pause, change/remove to resume\. Deployments: \`shared/managed\-agents\-scheduled\-deployments\.md\` § Deployment b

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Unrestricted Tool Access \(EA1\) \(medium\):** Excessive Agency: call any tool

**File:** shared/managed\-agents\-quickstarts/performance\-tuner\.md

**Line:** 52

**Source line:**  Give every function its own agent, have a second agent check every result, and send back whatever can still get better\.  Begin your first reply with the plan, before you call any tool: the functions 

**Suggested fix:** Skill grants unrestricted tool access without appropriate constraints\. An agent with unfettered tool access can perform arbitrary actions including file modification, network requests, and code execution\. Restrict tool access to only the tools required for the skill's stated purpose\. Use an explicit allowlist rather than granting blanket access\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Unrestricted Tool Access \(EA1\) \(medium\):** Excessive Agency: call any tool

**File:** shared/managed\-agents\-quickstarts/watchlist\-scanner\.md

**Line:** 58

**Source line:** Depth and cost\. Searches are what a scan costs, about 10 cents each\. \- Quick, the default: each scanner gets 3 searches and each reviewer 2, as hard limits, no other agent searches, and the reviewer c

**Suggested fix:** Skill grants unrestricted tool access without appropriate constraints\. An agent with unfettered tool access can perform arbitrary actions including file modification, network requests, and code execution\. Restrict tool access to only the tools required for the skill's stated purpose\. Use an explicit allowlist rather than granting blanket access\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Behavior Manipulation \(P4\) \(medium\):** Prompt Injection: never tell them

**File:** shared/managed\-agents\-quickstarts/watchlist\-scanner\.md

**Line:** 44

**Source line:**  You scan a stock watchlist and report what changed for each ticker: a positive, neutral or negative signal, the news behind it, and links to where it came from\.  This is research to help someone deci

**Suggested fix:** Subtle instructions detected that may alter agent decision\-making or introduce hidden biases\. Review content for implicit steering or bias\. Ensure instructions are explicit and align with the skill's stated purpose\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: curl \-fsSL https://api\.anthropic\.com/v1/deployments \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-H "anthropic\-beta: managed\-agents\-2026\-04\-01" \\   \-H "content\-typ

**File:** shared/managed\-agents\-scheduled\-deployments\.md

**Line:** 16

**Source line:** \- \`schedule\` takes a cron \`expression\` and an IANA \`timezone\`\. Minute\-level granularity is the maximum\.  \`\`\`bash curl \-fsSL https://api\.anthropic\.com/v1/deployments \\   \-H "x\-api\-key: $ANTHROPIC\_API\_K

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Sudo/Root Execution \(PE2\) \(medium\):** Privilege Escalation: sudo 

**File:** shared/managed\-agents\-self\-hosted\-sandboxes\.md

**Line:** 187

**Source line:** \*\*Prepare the host\.\*\* POSIX \(Linux/macOS\) only; a case\-sensitive filesystem is recommended\. Before starting the worker:  \`\`\`bash sudo mkdir \-p /mnt/memory &amp;&amp; sudo chown "$USER" /mnt/memory \`\`\`  Do \*\*n

**Suggested fix:** Commands invoke sudo or root privileges\. Verify this elevated access is necessary and justified\. Avoid sudo/root unless strictly required\. Prefer least\-privilege patterns\. If elevation is needed, document the justification and scope\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Sudo/Root Execution \(PE2\) \(medium\):** Privilege Escalation: sudo 

**File:** shared/managed\-agents\-self\-hosted\-sandboxes\.md

**Line:** 187

**Source line:** \*\*Prepare the host\.\*\* POSIX \(Linux/macOS\) only; a case\-sensitive filesystem is recommended\. Before starting the worker:  \`\`\`bash sudo mkdir \-p /mnt/memory &amp;&amp; sudo chown "$USER" /mnt/memory \`\`\`  Do \*\*n

**Suggested fix:** Commands invoke sudo or root privileges\. Verify this elevated access is necessary and justified\. Avoid sudo/root unless strictly required\. Prefer least\-privilege patterns\. If elevation is needed, document the justification and scope\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Sudo/Root Execution \(PE2\) \(medium\):** Privilege Escalation: sudo 

**File:** shared/model\-migration\.md

**Line:** 2369

**Source line:** truction, to the system prompt: \*"When you change code that can be run, built, or type\-checked, run a real check that exercises the change before reporting it done: the project's tests, type\-checker, 

**Suggested fix:** Commands invoke sudo or root privileges\. Verify this elevated access is necessary and justified\. Avoid sudo/root unless strictly required\. Prefer least\-privilege patterns\. If elevation is needed, document the justification and scope\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: Docker image references without a specific tag \(:latest is implicit\) or digest \(@​sha256:\.\.\.\) can be silently replaced by

**File:** shared/managed\-agents\-self\-hosted\-sandboxes\.md

**Line:** 199

**Suggested fix:** Docker image references without a specific tag \(:latest is implicit\) or digest \(@​sha256:\.\.\.\) can be silently replaced by a malicious image\. Pin the image: image:tag or image@​sha256:abc123

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.notion\.com/

**File:** shared/managed\-agents\-tools\.md

**Line:** 358

**Source line:**     "refresh": \{       "refresh\_token": "&lt;refresh token&gt;",       "client\_id": "&lt;your OAuth client\_id&gt;",       "token\_endpoint": "https://api\.notion\.com/v1/oauth/token",       "token\_endpoint\_auth": \{ 

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: ls can also live in your codebase\. When a session mounts a repository via the \`github\_repository\` resource \(see \`shared/managed\-agents\-environments\.md\` \-&gt; GitHub Repositories\), the repository's root \`

**File:** shared/managed\-agents\-tools\.md

**Line:** 483

**Source line:**  \#\#\# Skills from a GitHub repository  Skills can also live in your codebase\. When a session mounts a repository via the \`github\_repository\` resource \(see \`shared/managed\-agents\-environments\.md\` \-&gt; Git

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: ls in the following locations are not discoverable: a bare \`\.claude/skills/SKILL\.md\` \(no skill directory\), anything nested deeper \(\`\.claude/skills/tools/code\-review/SKILL\.md\`\), a \`skills/\` directory o

**File:** shared/managed\-agents\-tools\.md

**Line:** 485

**Source line:** \` resource \(see \`shared/managed\-agents\-environments\.md\` \-&gt; GitHub Repositories\), the repository's root \`\.claude/skills\` directory is scanned at session start, and each skill found becomes available to

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Skill Enumeration \(AS3\) \(medium\):** Agent Snooping: ls are agent instructions \- treat them as part of your trust boundary\.\*\* Anyone who can commit to a mounted repository \(a merged external PR, a compromised dependency, a contributor\) can add or edit \`

**File:** shared/managed\-agents\-tools\.md

**Line:** 487

**Source line:** /\`\*\* \- one directory level deep at the repository root\. Skills in the following locations are not discoverable: a bare \`\.claude/skills/SKILL\.md\` \(no skill directory\), anything nested deeper \(\`\.claude/

**Suggested fix:** Skill enumerates or reads other installed skills\. Access to other skills' SKILL\.md files or the skills directory reveals prompt instructions, capabilities, and secrets that should be invisible to peer skills\. Remove all code or instructions that list or read other skills' files or directories\. Skills should operate independently; cross\-skill access is a privilege escalation\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Whitespace Padding \(P9\) \(medium\):** Prompt Injection: U\+0020 x100

**File:** shared/model\-migration\.md

**Line:** 245

**Source line:**  \*\*Recommended starting points:\*\*  \| Workload                                          \| Start at       \| Notes                                                                                         

**Suggested fix:** Large whitespace padding was detected \(a block of blank lines or a long run of spaces\)\. This can push injected instructions below or to the right of the visible area so a human reviewer never sees them while the agent still reads them\. Manual review of the hidden content is recommended\. Remove the large whitespace padding \(blank\-line blocks or long space runs\) and review any content hidden below or to the right of it\. Keep skill files compact and reviewable so no instructions can be concealed off\-screen\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Whitespace Padding \(P9\) \(medium\):** Prompt Injection: U\+0020 x127

**File:** shared/model\-migration\.md

**Line:** 323

**Source line:**  Prefilled responses on the final assistant turn are no longer supported on either Opus 4\.6 or Sonnet 4\.6 \- both return a 400\. Adding assistant messages \*elsewhere\* in the conversation \(e\.g\., for few\-

**Suggested fix:** Large whitespace padding was detected \(a block of blank lines or a long run of spaces\)\. This can push injected instructions below or to the right of the visible area so a human reviewer never sees them while the agent still reads them\. Manual review of the hidden content is recommended\. Remove the large whitespace padding \(blank\-line blocks or long space runs\) and review any content hidden below or to the right of it\. Keep skill files compact and reviewable so no instructions can be concealed off\-screen\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: auto\-approve

**File:** shared/model\-migration\.md

**Line:** 854

**Source line:**  \#\#\# New API feature: mid\-session system prompts  You can deliver trusted instructions partway through a session by placing \`\{"role": "system", \.\.\.\}\` entries directly in the \`messages\` array \- without

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Unrestricted Tool Access \(EA1\) \(medium\):** Excessive Agency: call any tools

**File:** shared/model\-migration\.md

**Line:** 1850

**Source line:** fic details that would be hard to reconstruct \- names, numbers, dates, exact wording, links or references \- kept exactly\. Be complete on these even at the cost of length; keep everything else concise\.

**Suggested fix:** Skill grants unrestricted tool access without appropriate constraints\. An agent with unfettered tool access can perform arbitrary actions including file modification, network requests, and code execution\. Restrict tool access to only the tools required for the skill's stated purpose\. Use an explicit allowlist rather than granting blanket access\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Persistent Context Injection \(MP1\) \(medium\):** Memory Poisoning: a permanent rule

**File:** shared/prompt\-audit\.md

**Line:** 145

**Source line:** ng things the model already knows \| Every paragraph must justify its token cost; general programming knowledge doesn't \| Apply the Step 3 deletion rule paragraph by paragraph \| \| Wrong degrees of free

**Suggested fix:** Skill injects content designed to persist in agent memory or context across interactions\. Persistent injection can alter agent behavior long after the initial interaction\. Do not allow untrusted input to persist in agent memory or context\. Validate all content before storing and implement memory isolation between sessions\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: no verification

**File:** shared/prompt\-audit\.md

**Line:** 146

**Source line:** ose for fragile operations under\-constrains \| Match specificity to fragility: prose heuristics for open fields, exact commands \(\`do not modify this command\`\) only for narrow bridges \| \| The recency tr

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:35

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:128

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:464

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:552

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:601

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:602

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/tool\-use\-concepts\.md \(partial\) in SKILL\.md:606

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:59

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:64

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:204

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:207

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:209

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:212

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:213

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:217

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:221

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:225

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:255

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:258

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:264

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:268

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:269

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:327

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:412

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:523

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:535

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:537

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:539

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:541

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:591

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/model\-migration\.md \(partial\) in SKILL\.md:593

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/prompt\-audit\.md \(partial\) in SKILL\.md:59

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/prompt\-audit\.md \(partial\) in SKILL\.md:60

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/prompt\-audit\.md \(partial\) in SKILL\.md:545

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/models\.md \(partial\) in SKILL\.md:200

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/models\.md \(partial\) in SKILL\.md:229

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/anthropic\-cli\.md \(partial\) in SKILL\.md:244

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/anthropic\-cli\.md \(partial\) in SKILL\.md:434

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/anthropic\-cli\.md \(partial\) in SKILL\.md:442

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/managed\-agents\-multiagent\.md \(partial\) in SKILL\.md:446

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: shared/managed\-agents\-multiagent\.md \(partial\) in SKILL\.md:448

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: send the full conversation history in python/claude\-api/README\.md:334

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: send the full conversation history in typescript/claude\-api/README\.md:256

**Error:** \[SECURITY\-HIGH\] Anti\-Refusal: no warning in python/claude\-api/tool\-use\.md:68

**Error:** \[SECURITY\-HIGH\] Anti\-Refusal: no warning in typescript/claude\-api/tool\-use\.md:69

**Error:** \[SECURITY\-HIGH\] Tool Misuse: \| sudo  in shared/anthropic\-cli\.md:25

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: access token in shared/anthropic\-cli\.md:57

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: access token in shared/managed\-agents\-tools\.md:353

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: access token in shared/managed\-agents\-tools\.md:373

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: \.env  in shared/anthropic\-cli\.md:65

**Error:** \[SECURITY\-HIGH\] Excessive Agency: ant messages create \-\-model claude\-opus\-5\-5 \-\-max\-tokens 1024 \-\-message '\{role: user, content: "Hello"\}' in shared/anthropic\-cli\.md:85

**Error:** \[SECURITY\-HIGH\] Excessive Agency: ant messages create \-\-model claude\-opus\-5\-5 \-\-max\-tokens 1024 \\ in shared/anthropic\-cli\.md:154

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: Extract context in shared/live\-sources\.md:87

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: Extract context in shared/live\-sources\.md:89

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: Access Token in shared/managed\-agents\-environments\.md:133

**Error:** \[SECURITY\-HIGH\] Supply Chain: curl \| sh in shared/managed\-agents\-onboarding\-from\-url\.md:30

**Error:** \[SECURITY\-HIGH\] Tool Misuse: &amp;&amp; sudo in shared/managed\-agents\-self\-hosted\-sandboxes\.md:187

**Error:** \[SECURITY\-HIGH\] Tool Misuse: rm \-rf / in shared/managed\-agents\-tools\.md:144

**Error:** \[SECURITY\-HIGH\] Tool Misuse: rm \-rf /workspace/reports in shared/managed\-agents\-tools\.md:144

**Error:** \[SECURITY\-HIGH\] Tool Misuse: rm \-rf /workspace/reports" in shared/managed\-agents\-tools\.md:144

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: Access Tokens in shared/managed\-agents\-tools\.md:336

**Error:** \[SECURITY\-HIGH\] YARA Match: tools =; tools =; tools=; tools=; "tools":; tools":; "tools":; tools":; tools=; tools=; tools=; tools=; "tools":; tools":; tools:; tools:; tools:; parameters:; "description":; description":; "descript in shared/model\-migration\.md:406

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: send the conversation  in shared/model\-migration\.md:1446

**Error:** \[SECURITY\-HIGH\] Memory Poisoning: new name is in shared/preserved\-thinking\-migration/causes\.md:37

**Error:** \[SECURITY\-HIGH\] Agent Snooping: mcp\.json\`\) can hold secret in shared/prompt\-audit\.md:33

**Error:** \[SECURITY\-HIGH\] Excessive Agency: ant messages count\-tokens \-\-model claude\-opus\-5\-5 \\ in shared/token\-counting\.md:31

**Warning:** \[SECURITY\-MEDIUM\] MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\. in SKILL\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in SKILL\.md:71

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in SKILL\.md:591

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-onboarding\-from\-quickstart\.md:54

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-onboarding\-from\-quickstart\.md:57

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-onboarding\-from\-quickstart\.md:58

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-quickstarts/bug\-hunter\.md:74

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-quickstarts/explainer\-video\-maker\.md:70

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-quickstarts/performance\-tuner\.md:86

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/managed\-agents\-quickstarts/watchlist\-scanner\.md:69

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/model\-migration\.md:53

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/model\-migration\.md:1502

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without asking in shared/model\-migration\.md:1813

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: write \`claude\-fable\-5\-1\`, \`claude\-opus\-5\-5\`, \`claude\-opus\-5\`, or \`claude\-sonnet\-5\-5\` code, include the server\-side \`fallbacks\` parameter by default\*\* \(for \`claude\-sonnet\-5\-5\`, only the \`"default"\` for in SKILL\.md:209

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: don't ask the user in SKILL\.md:237

**Warning:** \[SECURITY\-MEDIUM\] Memory Poisoning: exceed context window in SKILL\.md:520

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: cURL / Raw HTTP  Use these examples when the user needs raw HTTP requests or is working in a language without an official SDK\.  \#\# Setup  \`\`\`bash export ANTHROPIC\_API\_KEY="your\-api\-key" \`\`\`  \-\-\-  \#\# B in curl/examples\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:16

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:37

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:63

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:102

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:127

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:165

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:192

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/examples\.md:217

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:24

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:38

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:66

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:85

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:99

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:130

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:153

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:166

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:171

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:183

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:200

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:225

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:229

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:240

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:260

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:278

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:294

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:303

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:312

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:321

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:335

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:341

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:352

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:362

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:384

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in curl/managed\-agents\.md:400

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in php/managed\-agents/README\.md:248

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in shared/admin\-api\.md:5

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in shared/anthropic\-cli\.md:58

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in shared/managed\-agents\-scheduled\-deployments\.md:16

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.anthropic\.com/ in shared/models\.md:35

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: curl https://api\.anthropic\.com/v1/messages \\   \-H "Content\-Type: application/json" \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-d '\{     "model": "claude\-opus\-5\-5 in curl/examples\.md:63

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: cURL / Raw HTTP  Use these examples when the user needs raw HTTP requests or is working without an SDK\.  \#\# Setup  \`\`\`bash export ANTHROPIC\_API\_KEY="your\-api\-key"  \# Common headers HEADERS=\(   \-H "Con in curl/managed\-agents\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: automatically run in go/claude\-api/tool\-use\.md:56

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: automatically run in python/claude\-api/tool\-use\.md:42

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in go/managed\-agents/README\.md:430

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in java/managed\-agents/README\.md:342

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in php/managed\-agents/README\.md:353

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in ruby/managed\-agents/README\.md:297

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in shared/managed\-agents\-api\-reference\.md:259

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in shared/managed\-agents\-environments\.md:154

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in shared/managed\-agents\-environments\.md:197

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.githubcopilot\.com/ in shared/managed\-agents\-quickstarts/incident\-commander\.md:31

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without checking in php/claude\-api/README\.md:69

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: without checking in shared/managed\-agents\-outcomes\.md:69

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: max\_retries=0 in python/claude\-api/README\.md:57

**Warning:** \[SECURITY\-MEDIUM\] Memory Poisoning: exceed the context window in shared/agent\-design\.md:80

**Warning:** \[SECURITY\-MEDIUM\] Privilege Escalation: sudo  in shared/anthropic\-cli\.md:25

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: curl https://api\.anthropic\.com/v1/messages \\   \-H "Authorization: Bearer $\(ant auth print\-credentials \-\-access\-token\)" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-H "anthropic\-beta: oauth\-2025\-04\-20"  in shared/anthropic\-cli\.md:58

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: skills/pr\-summary/SKILL\.md in shared/anthropic\-cli\.md:171

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: ls stored in its root \`\.claude/skills in shared/managed\-agents\-environments\.md:123

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: skills/brief\-format/SKILL\.md in shared/managed\-agents\-onboarding\-from\-url\.md:108

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: ls from a GitHub repository\) \- root \`\.claude/skills in shared/managed\-agents\-overview\.md:64

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: call any tool in shared/managed\-agents\-quickstarts/performance\-tuner\.md:52

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: call any tool in shared/managed\-agents\-quickstarts/watchlist\-scanner\.md:58

**Warning:** \[SECURITY\-MEDIUM\] Prompt Injection: never tell them in shared/managed\-agents\-quickstarts/watchlist\-scanner\.md:44

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: curl \-fsSL https://api\.anthropic\.com/v1/deployments \\   \-H "x\-api\-key: $ANTHROPIC\_API\_KEY" \\   \-H "anthropic\-version: 2023\-06\-01" \\   \-H "anthropic\-beta: managed\-agents\-2026\-04\-01" \\   \-H "content\-typ in shared/managed\-agents\-scheduled\-deployments\.md:16

**Warning:** \[SECURITY\-MEDIUM\] Privilege Escalation: sudo  in shared/managed\-agents\-self\-hosted\-sandboxes\.md:187

**Warning:** \[SECURITY\-MEDIUM\] Privilege Escalation: sudo  in shared/managed\-agents\-self\-hosted\-sandboxes\.md:187

**Warning:** \[SECURITY\-MEDIUM\] Privilege Escalation: sudo  in shared/model\-migration\.md:2369

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: Docker image references without a specific tag \(:latest is implicit\) or digest \(@​sha256:\.\.\.\) can be silently replaced by in shared/managed\-agents\-self\-hosted\-sandboxes\.md:199

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.notion\.com/ in shared/managed\-agents\-tools\.md:358

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: ls can also live in your codebase\. When a session mounts a repository via the \`github\_repository\` resource \(see \`shared/managed\-agents\-environments\.md\` \-&gt; GitHub Repositories\), the repository's root \` in shared/managed\-agents\-tools\.md:483

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: ls in the following locations are not discoverable: a bare \`\.claude/skills/SKILL\.md\` \(no skill directory\), anything nested deeper \(\`\.claude/skills/tools/code\-review/SKILL\.md\`\), a \`skills/\` directory o in shared/managed\-agents\-tools\.md:485

**Warning:** \[SECURITY\-MEDIUM\] Agent Snooping: ls are agent instructions \- treat them as part of your trust boundary\.\*\* Anyone who can commit to a mounted repository \(a merged external PR, a compromised dependency, a contributor\) can add or edit \` in shared/managed\-agents\-tools\.md:487

**Warning:** \[SECURITY\-MEDIUM\] Prompt Injection: U\+0020 x100 in shared/model\-migration\.md:245

**Warning:** \[SECURITY\-MEDIUM\] Prompt Injection: U\+0020 x127 in shared/model\-migration\.md:323

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: auto\-approve in shared/model\-migration\.md:854

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: call any tools in shared/model\-migration\.md:1850

**Warning:** \[SECURITY\-MEDIUM\] Memory Poisoning: a permanent rule in shared/prompt\-audit\.md:145

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: no verification in shared/prompt\-audit\.md:146

**Scanner message:** skillspector risk score: 100/100 \(CRITICAL\)

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 89 files for PII

**Evidence metadata:** \{"file\_count": 89\}

**Finding: emails \(high\):** Non\-placeholder email address: jane@​co\.com — 2 occurrences \(python/claude\-api/tool\-use\.md line 537; typescript/claude\-api/tool\-use\.md line 599\)

**File:** python/claude\-api/tool\-use\.md

**Line:** 537

**Source line:**         "content": "Extract: Jane Doe \(jane@​co\.com\) wants Enterprise, interested in API and SDKs, wants a demo\."

**Suggested fix:** Remove the address or use a placeholder like user@​example\.com

**Finding metadata:** \{"confidence": "high", "matched\_value": "jane@​co\.com", "occurrence\_count": 2, "occurrences": \[\{"file": "python/claude\-api/tool\-use\.md", "line": 537\}, \{"file": "typescript/claude\-api/tool\-use\.md", "line": 599\}\]\}

**Finding: emails \(high\):** Non\-placeholder email address: john@​co\.com

**File:** php/claude\-api/tool\-use\.md

**Line:** 174

**Source line:**     messages: \[\['role' =&gt; 'user', 'content' =&gt; 'Extract: John \(john@​co\.com\), Enterprise plan'\]\],

**Suggested fix:** Remove the address or use a placeholder like user@​example\.com

**Finding metadata:** \{"confidence": "high", "matched\_value": "john@​co\.com", "occurrence\_count": 1, "occurrences": \[\{"file": "php/claude\-api/tool\-use\.md", "line": 174\}\]\}

**Error:** \[PII\-HIGH\] Non\-placeholder email address: jane@​co\.com — 2 occurrences \(python/claude\-api/tool\-use\.md line 537; typescript/claude\-api/tool\-use\.md line 599\) in python/claude\-api/tool\-use\.md:537

**Error:** \[PII\-HIGH\] Non\-placeholder email address: john@​co\.com in php/claude\-api/tool\-use\.md:174

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 89 files for PII

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: semgrep:** Semgrep: No security issues found

**Finding: B310:blacklist \(medium\):** Audit url open for permitted schemes\. Allowing use of file:/ or custom schemes is often unexpected\. \(CWE\-22\)

**File:** /workspace/skills/claude\-api/shared/preserved\-thinking\-migration/drop\_block\_probe\.py

**Line:** 435

**Suggested fix:** Review blacklist \(B310\) \(CWE\-22\)

**Finding metadata:** \{"cwe": 22\}

**Error:** \[BANDIT\-MEDIUM\] Audit url open for permitted schemes\. Allowing use of file:/ or custom schemes is often unexpected\. \(CWE\-22\) in /workspace/skills/claude\-api/shared/preserved\-thinking\-migration/drop\_block\_probe\.py:435

**Scanner message:** Found 2 Python, 0 Shell, 0 JavaScript/TypeScript files

**Scanner message:** Bandit found: 0 HIGH, 1 MEDIUM, 0 LOW

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 86 markdown files for dead links

**Evidence metadata:** \{"file\_count": 86\}

**Evidence: dead\_links:** All relative links valid in 86 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 86\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 86 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 86 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 89 file\(s\)

**Evidence metadata:** \{"files\_scanned": 89\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 89 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 79\.8/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 79\.8, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(high\):** Name contains reserved word \(anthropic, claude\)

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Remove reserved words from skill name

**Finding metadata:** \{"deduction": 15, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(1068 chars, recommend 50\-150\)

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** Broad description without negative triggers may cause over\-triggering

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add boundary phrases like 'Do NOT use for\.\.\.'

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_efficiency \(medium\):** Large skill \(26279 tokens, recommended max &lt;5000\)\. Per agentskills\.io, SKILL\.md should be concise \(\~500 lines\) — large skill bodies increase token cost after invocation; long or unfocused top\-level descriptions can degrade agent routing accuracy

**File:** /workspace/skills/claude\-api/SKILL\.md

**Suggested fix:** Keep required sections concise; move detailed examples, reference material, and supporting docs to the references/ directory

**Finding metadata:** \{"deduction": 15, "dimension": "efficiency"\}

**Error:** \[QUALITY\-HIGH\] Name contains reserved word \(anthropic, claude\) in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(1068 chars, recommend 50\-150\) in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Broad description without negative triggers may cause over\-triggering in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/claude\-api/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Large skill \(26279 tokens, recommended max &lt;5000\)\. Per agentskills\.io, SKILL\.md should be concise \(\~500 lines\) — large skill bodies increase token cost after invocation; long or unfocused top\-level descriptions can degrade agent routing accuracy in /workspace/skills/claude\-api/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 79\.8/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/discernment\-nudge

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-008) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-008/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-008/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 85 | 0\.35 | 3 |
| discoverability | 55 | 0\.25 | 5 |
| reliability | 85 | 0\.25 | 3 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 7 | 1 | 4 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | FAIL | 0 | 1 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 11 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/discernment\-nudge/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'discernment\-nudge'

**Evidence metadata:** \{"description\_length": 983\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/discernment\-nudge/

**Evidence: naming\_convention:** Folder name 'discernment\-nudge' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 17\}

**Evidence: line\_count:** SKILL\.md within line limit \(209/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 209\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: name\_consistency:** Directory name matches frontmatter: 'discernment\-nudge'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/discernment\-nudge/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/discernment\-nudge/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'discernment\-nudge'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/discernment\-nudge/

**Scanner message:** \[OK\] naming\_convention: Folder name 'discernment\-nudge' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(209/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'discernment\-nudge'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Anti\-Refusal Statement \(AR1\) \(high\):** Anti\-Refusal: Always answer

**File:** SKILL\.md

**Line:** 191

**Source line:**  \#\# Output format  Always answer the question completely first\. The nudge comes after, and it should be easy to skip\.  The nudge is plain text: append it after a blank line at the end of

**Suggested fix:** Skill instructs the agent to never refuse or to always comply\. Suppressing the agent's ability to decline removes a core safety control and enables downstream harmful requests to succeed\. Remove any instruction telling the agent to never refuse or always comply\. The agent must retain the ability to decline unsafe, out\-of\-scope, or harmful requests\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Error:** \[SECURITY\-HIGH\] Anti\-Refusal: Always answer in SKILL\.md:191

**Scanner message:** skillspector found 1 issue\(s\) including critical/high severity

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 2 files for PII

**Evidence metadata:** \{"file\_count": 2\}

**Evidence: pii\_detection:** No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 2 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 2 file\(s\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 2 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 79\.8/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 79\.8, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(983 chars, recommend 50\-150\)

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Description contains vague words

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Be specific about what this skill does

**Finding metadata:** \{"deduction": 15, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Description uses first/second person

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Use third person: 'Processes files' not 'I can process'

**Finding metadata:** \{"deduction": 15, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** Broad description without negative triggers may cause over\-triggering

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add boundary phrases like 'Do NOT use for\.\.\.'

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/discernment\-nudge/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(983 chars, recommend 50\-150\) in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Description contains vague words in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Description uses first/second person in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Broad description without negative triggers may cause over\-triggering in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/discernment\-nudge/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/discernment\-nudge/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 79\.8/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/doc\-coauthoring

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-009) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-009/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-009/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 80 | 0\.35 | 4 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 75 | 0\.25 | 4 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 8 | 1 | 3 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 1 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 1 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 10 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/doc\-coauthoring/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'doc\-coauthoring'

**Evidence metadata:** \{"description\_length": 428\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/doc\-coauthoring/

**Evidence: naming\_convention:** Folder name 'doc\-coauthoring' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 15\}

**Evidence: line\_count:** SKILL\.md within line limit \(375/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 375\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: optional\_files:** Skill directory contains only expected files

**Evidence: name\_consistency:** Directory name matches frontmatter: 'doc\-coauthoring'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'doc\-coauthoring'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/doc\-coauthoring/

**Scanner message:** \[OK\] naming\_convention: Folder name 'doc\-coauthoring' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(375/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] optional\_files: Skill directory contains only expected files

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'doc\-coauthoring'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 1 files for PII

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: pii\_detection:** No PII detected in 1 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 1\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 1 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 1 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(not detected\)

**Evidence metadata:** \{"license\_status": "not\_detected"\}

**Warning:** No license information found \- manual review required\. Add a LICENSE file or 'license' field in frontmatter\.

**Scanner message:** No license detected in any tier

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(not detected\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 1 file\(s\)

**Evidence metadata:** \{"files\_scanned": 1\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 1 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 84\.2/100 \(Grade: B\)

**Evidence metadata:** \{"grade": "B", "overall\_score": 84\.2, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(low\):** No examples provided

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add example usage with code blocks

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(428 chars, recommend 50\-150\)

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No mention of error handling or validation

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Document expected errors and how to handle them

**Finding metadata:** \{"deduction": 10, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/doc\-coauthoring/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-LOW\] No examples provided in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(428 chars, recommend 50\-150\) in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No mention of error handling or validation in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/doc\-coauthoring/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/doc\-coauthoring/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 84\.2/100 \(Grade: B\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/docx

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-010) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-010/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-010/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 65 | 0\.35 | 5 |
| discoverability | 65 | 0\.25 | 4 |
| reliability | 80 | 0\.25 | 4 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 8 | 1 | 4 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 7 | 21 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | FAIL | 0 | 1 | 0 |
| Code Risk Analysis | FAIL | 1 | 1 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 13 |
| SCRIPT\_LINT | PASS | 0 | 0 | 8 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/docx/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'docx'

**Evidence metadata:** \{"description\_length": 835\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/docx/

**Evidence: naming\_convention:** Folder name 'docx' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 4\}

**Evidence: line\_count:** SKILL\.md within line limit \(91/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 91\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: optional\_files:** Found optional supporting files: scripts

**Evidence metadata:** \{"files\_found": \["scripts"\]\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'docx'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/docx/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/docx/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/docx/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/docx/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/docx/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'docx'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/docx/

**Scanner message:** \[OK\] naming\_convention: Folder name 'docx' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(91/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] optional\_files: Found optional supporting files: scripts

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'docx'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Tool Parameter Abuse \(TM1\) \(high\):** Tool Misuse: rm \-f \.\./out\.docx

**File:** SKILL\.md

**Line:** 56

**Source line:** find unpacked \-type l \-delete   \# strip symlink entries — docx from external parties is untrusted python scripts/merge\_runs\.py unpacked/   \# coalesce fragmented runs so text is findable \# edit unpacke

**Suggested fix:** Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Chaining Abuse \(TM2\) \(high\):** Tool Misuse: &amp;&amp; rm \-

**File:** SKILL\.md

**Line:** 56

**Source line:** find unpacked \-type l \-delete   \# strip symlink entries — docx from external parties is untrusted python scripts/merge\_runs\.py unpacked/   \# coalesce fragmented runs so text is findable \# edit unpacke

**Suggested fix:** Tool calls are chained to bypass individual safety checks or escalate capabilities beyond what any single tool call would allow\. Limit tool chaining depth and validate the output of each tool before passing it to the next\. Require explicit user approval for multi\-step chains\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Hidden Instructions \(P2\) \(high\):** Prompt Injection: ﻿

**File:** scripts/office/schemas/ecma/fouth\-edition/opc\-contentTypes\.xsd

**Line:** 1

**Source line:** ﻿&lt;?xml version="1\.0" encoding="UTF\-8" standalone="no"?&gt; &lt;xs:schema xmlns="http://schemas\.openxmlformats\.org/package/2006/content\-types"   xmlns:xs="http://www\.w3\.org/2001/XMLSchema"   targetNamespace=

**Suggested fix:** Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Hidden Instructions \(P2\) \(high\):** Prompt Injection: ﻿

**File:** scripts/office/schemas/ecma/fouth\-edition/opc\-coreProperties\.xsd

**Line:** 1

**Source line:** ﻿&lt;?xml version="1\.0" encoding="UTF\-8"?&gt; &lt;xs:schema targetNamespace="http://schemas\.openxmlformats\.org/package/2006/metadata/core\-properties"   xmlns="http://schemas\.openxmlformats\.org/package/2006/met

**Suggested fix:** Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Hidden Instructions \(P2\) \(high\):** Prompt Injection: ﻿

**File:** scripts/office/schemas/ecma/fouth\-edition/opc\-relationships\.xsd

**Line:** 1

**Source line:** ﻿&lt;?xml version="1\.0" encoding="UTF\-8" standalone="no"?&gt; &lt;xsd:schema xmlns="http://schemas\.openxmlformats\.org/package/2006/relationships"   xmlns:xsd="http://www\.w3\.org/2001/XMLSchema"   targetNamespac

**Suggested fix:** Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Env Variable Harvesting \(E2\) \(high\):** Data Exfiltration: os\.environ\.copy\(\)

**File:** scripts/office/soffice\.py

**Line:** 28

**Source line:**   def get\_soffice\_env\(\) \-&gt; dict:     env = os\.environ\.copy\(\)     env\["SAL\_USE\_VCLPLUGIN"\] = "svp"      if \_needs\_shim\(\):

**Suggested fix:** Code enumerates, copies, or searches environment variables for secrets\. Bulk environment access can collect credentials unrelated to the skill's stated purpose\. Read only explicitly required environment variables by name\. Avoid enumerating or copying the full environment, and never log or transmit credentials to untrusted destinations\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Unknown \(LP3\) \(medium\):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(             cmd,             capture\_output=True,             text=True,             timeout=30,             check=False,             env=get\_soffice\_env\(\),         \)

**File:** scripts/accept\_changes\.py

**Line:** 68

**Source line:**     \]      try:         result = subprocess\.run\(             cmd,             capture\_output=True,             text=True,

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(             \[                 "soffice",                 "\-\-headless",                 f"\-env:UserInstallation=file://\{LIBREOFFICE\_PROFILE\}",                 "\-\-terminate\_after\_init", 

**File:** scripts/accept\_changes\.py

**Line:** 99

**Source line:**         return True      if not macro\_dir\.exists\(\):         subprocess\.run\(             \[                 "soffice",                 "\-\-headless",

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unsafe Defaults \(TM3\) \(medium\):** Tool Misuse: mode = 0o666

**File:** scripts/office/helpers/\_\_init\_\_\.py

**Line:** 106

**Source line:**         else:             umask = os\.umask\(0\)             os\.umask\(umask\)             mode = 0o666 &amp; \~umask         os\.chmod\(tmp\_out, mode\)         os\.replace\(tmp\_out, out\_path\)     finally:

**Suggested fix:** Tool defaults are unsafe or overly permissive \(e\.g\. disabled TLS verification, no authentication, world\-writable permissions\)\. Unsafe defaults widen the attack surface\. Override unsafe defaults with secure settings \(verify=True, auth required, restrictive permissions\)\. Review and harden all tool configurations\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 1455

**Source line:**     &lt;/xsd:sequence&gt;     &lt;xsd:attribute name="pos" type="ST\_PositiveFixedPercentage" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_GradientStopList"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:e

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 1462

**Source line:**   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_GradientFillProperties"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:element name="gsLst" type="CT\_GradientStopList" minOccurs="0" maxOccurs="1"/&gt;       &lt;xsd:group r

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 2189

**Source line:**     &lt;xsd:attribute name="d" type="ST\_PositivePercentage" use="required"/&gt;     &lt;xsd:attribute name="sp" type="ST\_PositivePercentage" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_Da

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 2197

**Source line:**   &lt;xsd:group name="EG\_LineDashProperties"&gt;     &lt;xsd:choice&gt;       &lt;xsd:element name="prstDash" type="CT\_PresetLineDashProperties" minOccurs="1" maxOccurs="1"/&gt;       &lt;xsd:element name="custDash" type=

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 2992

**Source line:**     &lt;xsd:attribute name="pos" type="ST\_Coordinate32" use="optional"/&gt;     &lt;xsd:attribute name="algn" type="ST\_TextTabAlignType" use="optional"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_TextTa

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 3043

**Source line:**       &lt;xsd:group ref="EG\_TextBulletSize" minOccurs="0" maxOccurs="1"/&gt;       &lt;xsd:group ref="EG\_TextBulletTypeface" minOccurs="0" maxOccurs="1"/&gt;       &lt;xsd:group ref="EG\_TextBullet" minOccurs="0" max

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 730

**Source line:**     &lt;xsd:attribute name="st" type="ST\_Index" use="required"/&gt;     &lt;xsd:attribute name="end" type="ST\_Index" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_SlideRelationshipListEntry

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 733

**Source line:**   &lt;xsd:complexType name="CT\_SlideRelationshipListEntry"&gt;     &lt;xsd:attribute ref="r:id" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_SlideRelationshipList"&gt;     &lt;xsd:sequence&gt;     

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 735

**Source line:**   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_SlideRelationshipList"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:element name="sld" type="CT\_SlideRelationshipListEntry" minOccurs="0"         maxOccurs="unbounde

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 950

**Source line:**   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_CustomShow"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:element name="sldLst" type="CT\_SlideRelationshipList" minOccurs="1" maxOccurs="1"/&gt;       &lt;xsd:element name=

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/microsoft/wml\-2010\.xsd

**Line:** 181

**Source line:**      &lt;/xsd:sequence&gt;      &lt;xsd:attribute name="pos" type="a:ST\_PositiveFixedPercentage" use="required"/&gt;    &lt;/xsd:complexType&gt;    &lt;xsd:complexType name="CT\_GradientStopList"&gt;      &lt;xsd:sequence&gt;      

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/microsoft/wml\-2010\.xsd

**Line:** 209

**Source line:**    &lt;/xsd:complexType&gt;    &lt;xsd:complexType name="CT\_GradientFillProperties"&gt;      &lt;xsd:sequence&gt;        &lt;xsd:element name="gsLst" type="CT\_GradientStopList" minOccurs="0"/&gt;        &lt;xsd:group ref="EG\_Sh

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(\["soffice"\] \+ args, env=get\_soffice\_env\(\), \*\*kwargs\)

**File:** scripts/office/soffice\.py

**Line:** 46

**Source line:**                 tempfile\.TemporaryDirectory\(prefix="lo\_profile\_", ignore\_cleanup\_errors=True\)             \)             args = \[f"\-env:UserInstallation=\{Path\(profile\)\.as\_uri\(\)\}"\] \+ args         return

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(         \["gcc", "\-shared", "\-fPIC", "\-o", str\(\_SHIM\_SO\), str\(src\), "\-ldl"\],         check=True,         capture\_output=True,     \)

**File:** scripts/office/soffice\.py

**Line:** 68

**Source line:**      src = Path\(tempfile\.gettempdir\(\)\) / "lo\_socket\_shim\.c"     src\.write\_text\(\_SHIM\_SOURCE\)     subprocess\.run\(         \["gcc", "\-shared", "\-fPIC", "\-o", str\(\_SHIM\_SO\), str\(src\), "\-ldl"\],         che

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-\-word\-diff\-regex=\.",        

**File:** scripts/office/validators/redlining\.py

**Line:** 192

**Source line:**                 original\_file\.write\_text\(original\_text, encoding="utf\-8"\)                 modified\_file\.write\_text\(modified\_text, encoding="utf\-8"\)                  result = subprocess\.run\(           

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-U0",                        

**File:** scripts/office/validators/redlining\.py

**Line:** 221

**Source line:**                     if content\_lines:                         return "\\n"\.join\(content\_lines\)                  result = subprocess\.run\(                     \[                         "git",            

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Overly Broad Trigger \(TR1\) \(low\):** Trigger Abuse: Overly Broad Trigger: description clause 'If the user asks for a 'report', 'memo', 'letter', 'template', or similar deli

**File:** SKILL\.md

**Line:** 2

**Suggested fix:** Overly Broad Trigger: description clause 'If the user asks for a 'report', 'memo', 'letter', 'template', or similar deliverable as a Word or' activates on 'a', a common word that will activate in many unintended contexts Use specific, narrow trigger patterns that match only the skill's intended use case\. Avoid single\-word or common\-phrase triggers\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Error:** \[SECURITY\-HIGH\] Tool Misuse: rm \-f \.\./out\.docx in SKILL\.md:56

**Error:** \[SECURITY\-HIGH\] Tool Misuse: &amp;&amp; rm \- in SKILL\.md:56

**Error:** \[SECURITY\-HIGH\] Prompt Injection: ﻿ in scripts/office/schemas/ecma/fouth\-edition/opc\-contentTypes\.xsd:1

**Error:** \[SECURITY\-HIGH\] Prompt Injection: ﻿ in scripts/office/schemas/ecma/fouth\-edition/opc\-coreProperties\.xsd:1

**Error:** \[SECURITY\-HIGH\] Prompt Injection: ﻿ in scripts/office/schemas/ecma/fouth\-edition/opc\-relationships\.xsd:1

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: os\.environ\.copy\(\) in scripts/office/soffice\.py:28

**Warning:** \[SECURITY\-MEDIUM\] MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\. in SKILL\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(             cmd,             capture\_output=True,             text=True,             timeout=30,             check=False,             env=get\_soffice\_env\(\),         \) in scripts/accept\_changes\.py:68

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(             \[                 "soffice",                 "\-\-headless",                 f"\-env:UserInstallation=file://\{LIBREOFFICE\_PROFILE\}",                 "\-\-terminate\_after\_init",  in scripts/accept\_changes\.py:99

**Warning:** \[SECURITY\-MEDIUM\] Tool Misuse: mode = 0o666 in scripts/office/helpers/\_\_init\_\_\.py:106

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:1455

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:1462

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:2189

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:2197

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:2992

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:3043

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:730

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:733

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:735

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:950

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/microsoft/wml\-2010\.xsd:181

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/microsoft/wml\-2010\.xsd:209

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(\["soffice"\] \+ args, env=get\_soffice\_env\(\), \*\*kwargs\) in scripts/office/soffice\.py:46

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(         \["gcc", "\-shared", "\-fPIC", "\-o", str\(\_SHIM\_SO\), str\(src\), "\-ldl"\],         check=True,         capture\_output=True,     \) in scripts/office/soffice\.py:68

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-\-word\-diff\-regex=\.",         in scripts/office/validators/redlining\.py:192

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-U0",                         in scripts/office/validators/redlining\.py:221

**Warning:** \[SECURITY\-LOW\] Trigger Abuse: Overly Broad Trigger: description clause 'If the user asks for a 'report', 'memo', 'letter', 'template', or similar deli in SKILL\.md:2

**Scanner message:** skillspector risk score: 100/100 \(CRITICAL\)

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 17 files for PII

**Evidence metadata:** \{"file\_count": 17\}

**Evidence: pii\_detection:** No PII detected in 17 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 17\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 17 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 17 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Finding: blocked\_license \(critical\):** License 'Proprietary' is not allowed \(restrictive/copyleft\)

**File:** LICENSE\.txt

**Suggested fix:** This asset uses a restrictive license that is not permitted\. Contact the asset owner about re\-licensing, or find an alternative\.

**Error:** \[LICENSE\-CRITICAL\] License 'Proprietary' is not allowed \(restrictive/copyleft\) in LICENSE\.txt

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Proprietary\. LICENSE\.txt has complete terms'

### Code Risk Analysis — evidence

**Evidence: semgrep:** Semgrep: No security issues found

**Finding: B108:hardcoded\_tmp\_directory \(medium\):** Probable insecure usage of temp file/directory\. \(CWE\-377\)

**File:** /workspace/skills/docx/scripts/accept\_changes\.py

**Line:** 16

**Suggested fix:** Review hardcoded\_tmp\_directory \(B108\) \(CWE\-377\)

**Finding metadata:** \{"cwe": 377\}

**Error:** \[BANDIT\-MEDIUM\] Probable insecure usage of temp file/directory\. \(CWE\-377\) in /workspace/skills/docx/scripts/accept\_changes\.py:16

**Scanner message:** Found 15 Python, 0 Shell, 0 JavaScript/TypeScript files

**Scanner message:** Bandit found: 0 HIGH, 1 MEDIUM, 0 LOW

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 17 file\(s\)

**Evidence metadata:** \{"files\_scanned": 17\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 17 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 74\.0/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 74\.0, "skill\_type": "script\-based"\}

**Finding: quality\_correctness \(medium\):** No documented scripts in table format

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add '\#\# Available Scripts' with table: \| Script \| Purpose \| Arguments \|

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** Instructions don't mention 'run\_script'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add explicit run\_script\(\) call examples

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(835 chars, recommend 50\-150\)

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Description contains vague words

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Be specific about what this skill does

**Finding metadata:** \{"deduction": 15, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Skill name very short: 'docx'

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Use descriptive names like 'crypto\-utils' not 'crypto'

**Finding metadata:** \{"deduction": 10, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** Scripts may lack error handling: \_\_init\_\_\.py

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Scripts should handle errors explicitly

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/docx/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-MEDIUM\] No documented scripts in table format in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Instructions don't mention 'run\_script' in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(835 chars, recommend 50\-150\) in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Description contains vague words in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Skill name very short: 'docx' in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Scripts may lack error handling: \_\_init\_\_\.py in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/docx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/docx/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 74\.0/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Finding: flat\_script \(medium\):** \_\_init\_\_\.py has no function definitions \(flat script\)

**File:** /workspace/skills/docx/scripts/\_\_init\_\_\.py

**Suggested fix:** Wrap logic in functions for maintainability and testability

**Finding: missing\_shebang \(low\):** \_\_init\_\_\.py missing shebang line

**File:** /workspace/skills/docx/scripts/\_\_init\_\_\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: no\_input\_validation \(low\):** \_\_init\_\_\.py may lack input validation

**File:** /workspace/skills/docx/scripts/\_\_init\_\_\.py

**Suggested fix:** Add argument checks and raise descriptive errors

**Finding: magic\_numbers \(low\):** accept\_changes\.py contains magic numbers

**File:** /workspace/skills/docx/scripts/accept\_changes\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** accept\_changes\.py missing shebang line

**File:** /workspace/skills/docx/scripts/accept\_changes\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** comment\.py contains magic numbers

**File:** /workspace/skills/docx/scripts/comment\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** comment\.py missing shebang line

**File:** /workspace/skills/docx/scripts/comment\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: missing\_shebang \(low\):** merge\_runs\.py missing shebang line

**File:** /workspace/skills/docx/scripts/merge\_runs\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Warning:** \[SCRIPT\_LINT\-MEDIUM\] \_\_init\_\_\.py has no function definitions \(flat script\) in /workspace/skills/docx/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] \_\_init\_\_\.py missing shebang line in /workspace/skills/docx/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] \_\_init\_\_\.py may lack input validation in /workspace/skills/docx/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] accept\_changes\.py contains magic numbers in /workspace/skills/docx/scripts/accept\_changes\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] accept\_changes\.py missing shebang line in /workspace/skills/docx/scripts/accept\_changes\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] comment\.py contains magic numbers in /workspace/skills/docx/scripts/comment\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] comment\.py missing shebang line in /workspace/skills/docx/scripts/comment\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] merge\_runs\.py missing shebang line in /workspace/skills/docx/scripts/merge\_runs\.py

## skills/frontend\-design

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-011) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-011/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-011/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 80 | 0\.35 | 4 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 85 | 0\.25 | 3 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 7 | 1 | 4 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | FAIL | 0 | 1 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 9 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/frontend\-design/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'frontend\-design'

**Evidence metadata:** \{"description\_length": 204\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/frontend\-design/

**Evidence: naming\_convention:** Folder name 'frontend\-design' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 15\}

**Evidence: line\_count:** SKILL\.md within line limit \(71/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 71\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: name\_consistency:** Directory name matches frontmatter: 'frontend\-design'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/frontend\-design/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/frontend\-design/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'frontend\-design'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/frontend\-design/

**Scanner message:** \[OK\] naming\_convention: Folder name 'frontend\-design' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(71/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'frontend\-design'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Anti\-Refusal Statement \(AR2\) \(high\):** Anti\-Refusal: don't apologize

**File:** SKILL\.md

**Line:** 69

**Source line:**  Use active voice as default\. A CTA says exactly what happens when it is used: "Save changes," not "Submit\." An action keeps the same name through the whole flow, so the button that says "Publish" pro

**Suggested fix:** Skill instructs the agent to omit warnings, disclaimers, or ethical commentary\. Stripping safety caveats hides risk from the user and is a common jailbreak preamble\. Remove instructions that suppress warnings, disclaimers, or ethical commentary\. Let the agent surface safety\-relevant caveats to the user\.

**Finding metadata:** \{"skillspector\_confidence": 0\.55\}

**Error:** \[SECURITY\-HIGH\] Anti\-Refusal: don't apologize in SKILL\.md:69

**Scanner message:** skillspector found 1 issue\(s\) including critical/high severity

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 2 files for PII

**Evidence metadata:** \{"file\_count": 2\}

**Evidence: pii\_detection:** No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 2 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 2 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 2 file\(s\)

**Evidence metadata:** \{"files\_scanned": 2\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 2 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 86\.8/100 \(Grade: B\)

**Evidence metadata:** \{"grade": "B", "overall\_score": 86\.8, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(low\):** No examples provided

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add example usage with code blocks

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(204 chars, recommend 50\-150\)

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/frontend\-design/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-LOW\] No examples provided in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(204 chars, recommend 50\-150\) in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/frontend\-design/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/frontend\-design/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 86\.8/100 \(Grade: B\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/internal\-comms

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-012) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-012/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-012/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 80 | 0\.35 | 4 |
| discoverability | 70 | 0\.25 | 4 |
| reliability | 75 | 0\.25 | 4 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 6 | 2 | 5 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | PASS | 1 | 0 | 0 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | NOT APPLICABLE | 1 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 12 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/internal\-comms/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'internal\-comms'

**Evidence metadata:** \{"description\_length": 329\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/internal\-comms/

**Evidence: naming\_convention:** Folder name 'internal\-comms' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 14\}

**Evidence: line\_count:** SKILL\.md within line limit \(32/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 32\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'internal\-comms'

**Finding: body\_heading \(high\):** Missing top\-level heading \(\# Title\) in SKILL\.md body

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add a top\-level heading after the frontmatter, e\.g\. '\# My Skill'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'examples' in skill root

**File:** /workspace/skills/internal\-comms/examples

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/internal\-comms/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Missing top\-level heading \(\# Title\) in SKILL\.md body in /workspace/skills/internal\-comms/SKILL\.md

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'examples' in skill root in /workspace/skills/internal\-comms/examples

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/internal\-comms/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'internal\-comms'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/internal\-comms/

**Scanner message:** \[OK\] naming\_convention: Folder name 'internal\-comms' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(32/500\)

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'internal\-comms'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Evidence: skillspector:** No security vulnerabilities detected \(secrets, API keys, credentials\)

**Scanner message:** \[OK\] skillspector: No security vulnerabilities detected \(secrets, API keys, credentials\)

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 6 files for PII

**Evidence metadata:** \{"file\_count": 6\}

**Evidence: pii\_detection:** No PII detected in 6 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 6\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 6 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 6 files \(emails, SSNs, phone numbers, paths\)

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: code\_file\_discovery:** No code files found \- code risk analysis is not applicable

**Evidence metadata:** \{"file\_counts": \{"js": 0, "py": 0, "sh": 0\}\}

**Scanner message:** \[OK\] code\_file\_discovery: No code files found \- code risk analysis is not applicable

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 5 markdown files for dead links

**Evidence metadata:** \{"file\_count": 5\}

**Evidence: dead\_links:** All relative links valid in 5 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 5\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 5 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 5 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 6 file\(s\)

**Evidence metadata:** \{"files\_scanned": 6\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 6 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 79\.2/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 79\.2, "skill\_type": "guide\-only"\}

**Finding: quality\_correctness \(low\):** No examples provided

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add example usage with code blocks

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(329 chars, recommend 50\-150\)

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Description uses first/second person

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Use third person: 'Processes files' not 'I can process'

**Finding metadata:** \{"deduction": 15, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** Broad description without negative triggers may cause over\-triggering

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add boundary phrases like 'Do NOT use for\.\.\.'

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No mention of error handling or validation

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Document expected errors and how to handle them

**Finding metadata:** \{"deduction": 10, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/internal\-comms/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-LOW\] No examples provided in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(329 chars, recommend 50\-150\) in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Description uses first/second person in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Broad description without negative triggers may cause over\-triggering in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No mention of error handling or validation in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/internal\-comms/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/internal\-comms/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 79\.2/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Evidence: lint:** No scripts/ or tools/ directory found

**Scanner message:** \[OK\] lint: No scripts/ or tools/ directory found

## skills/mcp\-builder

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-013) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-013/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-013/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 65 | 0\.35 | 5 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 85 | 0\.25 | 3 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 8 | 1 | 5 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 10 | 16 |
| PII Scan | FAIL | 1 | 1 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | FAIL | 1 | 1 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 10 |
| SCRIPT\_LINT | PASS | 0 | 0 | 4 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/mcp\-builder/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'mcp\-builder'

**Evidence metadata:** \{"description\_length": 277\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/mcp\-builder/

**Evidence: naming\_convention:** Folder name 'mcp\-builder' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 11\}

**Evidence: line\_count:** SKILL\.md within line limit \(252/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 252\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: optional\_files:** Found optional supporting files: scripts

**Evidence metadata:** \{"files\_found": \["scripts"\]\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'mcp\-builder'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'reference' in skill root

**File:** /workspace/skills/mcp\-builder/reference

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/mcp\-builder/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'reference' in skill root in /workspace/skills/mcp\-builder/reference

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/mcp\-builder/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'mcp\-builder'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/mcp\-builder/

**Scanner message:** \[OK\] naming\_convention: Folder name 'mcp\-builder' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(252/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] optional\_files: Found optional supporting files: scripts

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'mcp\-builder'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\)

**File:** SKILL\.md

**Line:** 71

**Source line:** \- \[⚡ TypeScript Guide \(v2\)\]\(\./reference/node\_mcp\_server\_v2\.md\) \- TypeScript patterns and examples

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\)

**File:** SKILL\.md

**Line:** 93

**Source line:** \- \[⚡ TypeScript Guide \(v2\)\]\(\./reference/node\_mcp\_server\_v2\.md\) \- Project structure, package\.json, tsconfig\.json \(\[v1\]\(\./reference/node\_mcp\_server\.md\) for existi

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\)

**File:** SKILL\.md

**Line:** 151

**Source line:** \- v2 projects: run the self\-check script from the \[v2 guide\]\(\./reference/node\_mcp\_server\_v2\.md\#verify\-your\-server\) against the built server

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\)

**File:** SKILL\.md

**Line:** 235

**Source line:** \- \[⚡ TypeScript Implementation Guide \(SDK v2\)\]\(\./reference/node\_mcp\_server\_v2\.md\) \- Complete TypeScript guide for \`@​modelcontextprotocol/server\` with:

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\.md \(partial\)

**File:** SKILL\.md

**Line:** 72

**Source line:** lcontextprotocol/typescript\-sdk/v1\.x/README\.md\` and the \[TypeScript Guide \(v1\)\]\(\./reference/node\_mcp\_server\.md\)

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\.md \(partial\)

**File:** SKILL\.md

**Line:** 93

**Source line:** e/node\_mcp\_server\_v2\.md\) \- Project structure, package\.json, tsconfig\.json \(\[v1\]\(\./reference/node\_mcp\_server\.md\) for existing v1 projects\)

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: reference/node\_mcp\_server\.md \(partial\)

**File:** SKILL\.md

**Line:** 244

**Source line:** \- \[⚡ TypeScript Implementation Guide \(SDK v1\)\]\(\./reference/node\_mcp\_server\.md\) \- The equivalent guide for existing \`@​modelcontextprotocol/sdk\` projects

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Review the target's analysis\-completeness ledger and resolve all limitations\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: External Model or Provider Selection \(EA5\) \(high\):** Excessive Agency: \-m, \-\-model           Claude model to use \(default: claude\-3\-7\-sonnet\-20250219\)

**File:** reference/evaluation\.md

**Line:** 488

**Source line:** optional arguments:   \-h, \-\-help            Show help message   \-t, \-\-transport       Transport type: stdio, sse, or http \(default: stdio\)   \-m, \-\-model           Claude model to use \(default: claude\-

**Suggested fix:** Skill selects an external model or provider that may use a different account or billing plan than the operator expects\. Undisclosed model switches can cause unexpected cost or quota consumption\. Remove the model/provider override or disclose it prominently and require explicit operator approval before invoking an external coding CLI or billed model\.

**Finding metadata:** \{"skillspector\_confidence": 0\.9\}

**Finding: Credential Access \(PE3\) \(high\):** Privilege Escalation: access tokens

**File:** reference/mcp\_best\_practices\.md

**Line:** 158

**Source line:**  \*\*OAuth 2\.1\*\*: \- Use secure OAuth 2\.1 with certificates from recognized authorities \- Validate access tokens before processing requests \- Only accept tokens specifically intended for your server  \*\*A

**Suggested fix:** Code accesses credential files \(SSH keys, AWS credentials, etc\.\)\. This could indicate credential theft attempts\. Remove references to credential paths\. Use environment variables or secrets managers\. For docs, use placeholder paths \(e\.g\., /path/to/config\)\. Never load \.env or token files in production code paths\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(LP3\) \(medium\):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub

**File:** SKILL\.md

**Line:** 64

**Suggested fix:** npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and publishes a malicious update\. Pin the version: npx @​scope/server@​1\.2\.3

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub

**File:** SKILL\.md

**Line:** 66

**Suggested fix:** npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and publishes a malicious update\. Pin the version: npx @​scope/server@​1\.2\.3

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub

**File:** reference/node\_mcp\_server\_v2\.md

**Line:** 712

**Suggested fix:** npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and publishes a malicious update\. Pin the version: npx @​scope/server@​1\.2\.3

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub

**File:** SKILL\.md

**Line:** 152

**Suggested fix:** npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and publishes a malicious update\. Pin the version: npx @​scope/server@​1\.2\.3

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub

**File:** reference/node\_mcp\_server\_v2\.md

**Line:** 684

**Suggested fix:** npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and publishes a malicious update\. Pin the version: npx @​scope/server@​1\.2\.3

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unrestricted Tool Access \(EA1\) \(medium\):** Excessive Agency: call any tools

**File:** reference/evaluation\.md

**Line:** 205

**Source line:** After understanding the API and tools, USE the MCP server tools: \- Inspect content using READ\-ONLY and NON\-DESTRUCTIVE operations ONLY \- Goal: identify specific content \(e\.g\., users, channels, message

**Suggested fix:** Skill grants unrestricted tool access without appropriate constraints\. An agent with unfettered tool access can perform arbitrary actions including file modification, network requests, and code execution\. Restrict tool access to only the tools required for the skill's stated purpose\. Use an explicit allowlist rather than granting blanket access\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.example\.com/

**File:** reference/node\_mcp\_server\.md

**Line:** 603

**Source line:** import axios, \{ AxiosError \} from "axios";  // Constants const API\_BASE\_URL = "https://api\.example\.com/v1"; const CHARACTER\_LIMIT = 25000;  // Enums

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.example\.com/

**File:** reference/node\_mcp\_server\_v2\.md

**Line:** 294

**Source line:** import \{ serveStdio \} from "@​modelcontextprotocol/server/stdio"; import \* as z from "zod/v4";  const API\_BASE\_URL = "https://api\.example\.com/v1"; const API\_KEY = process\.env\.EXAMPLE\_API\_KEY; const CHA

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: External Transmission \(E1\) \(medium\):** Data Exfiltration: https://api\.example\.com/

**File:** reference/python\_mcp\_server\.md

**Line:** 353

**Source line:** mcp = FastMCP\("example\_mcp"\)  \# Constants API\_BASE\_URL = "https://api\.example\.com/v1"  \# Enums class ResponseFormat\(str, Enum\):

**Suggested fix:** Data is being sent to an external URL\. This could be legitimate telemetry or data exfiltration\. Manual review is recommended\. Verify the destination URL is trusted and necessary\. Remove or replace with documented APIs\. Ensure no secrets, tokens, or PII are transmitted\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: Autonomous Decision Making \(EA2\) \(medium\):** Excessive Agency: auto\-approve

**File:** reference/node\_mcp\_server\_v2\.md

**Line:** 193

**Source line:**  \#\#\# Annotations  Annotations are hints for clients, for example to auto\-approve read\-only tools or to confirm destructive ones\. They never change how the SDK runs the tool\.  \| Annotation \| Set to \`tr

**Suggested fix:** Skill enables autonomous high\-impact decisions without human\-in\-the\-loop verification\. Critical operations \(destructive commands, financial transactions, data deletion\) should require explicit user confirmation\. Add human\-in\-the\-loop confirmation for destructive, irreversible, or high\-impact operations\. Never auto\-execute commands that modify files, send data, or alter system state\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Unknown \(RP1\) \(medium\):** MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub

**File:** reference/node\_mcp\_server\_v2\.md

**Line:** 714

**Suggested fix:** npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and publishes a malicious update\. Pin the version: npx @​scope/server@​1\.2\.3

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unpinned Dependencies \(SC1\) \(low\):** Supply Chain: anthropic&gt;=0\.39\.0

**File:** scripts/requirements\.txt

**Line:** 1

**Source line:** anthropic&gt;=0\.39\.0 mcp&gt;=1\.1\.0

**Suggested fix:** Dependencies lack version pinning, allowing potential malicious package updates\. Consider pinning versions\. Pin all dependency versions in requirements\.txt or pyproject\.toml\. Use exact versions \(==\) or compatible ranges\. Run pip\-audit regularly\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: Unverifiable Dependency: anthropic has 4 known advisory\(ies\) \(CVE\-2026\-34450 \(Claude SDK for Python has Insecure Default File Permissions in Local Filesystem \); CVE\-2026\-34452 \(Claude SDK for Python: Memory Tool Path Validation Race Condition Allows Sandbox\); CVE\-2026\-34450 \(The Claude SDK for Python provides access to the Claude API from Python applicat\) \+1 more\), but the manifest does not pin a version, so it is unknown whether the installed release is affected \(SC4\) \(low\):** Supply Chain: anthropic

**File:** scripts/requirements\.txt

**Line:** 1

**Suggested fix:** Dependency has known vulnerabilities \(CVEs\)\. Using packages with unpatched security flaws exposes the environment to known exploits\. Update the dependency to a patched version that addresses the known CVE\. Check OSV \(osv\.dev\) or NVD for details on the vulnerability\.

**Finding metadata:** \{"skillspector\_confidence": 0\.4\}

**Finding: Unpinned Dependencies \(SC1\) \(low\):** Supply Chain: mcp&gt;=1\.1\.0 

**File:** scripts/requirements\.txt

**Line:** 2

**Source line:** anthropic&gt;=0\.39\.0 mcp&gt;=1\.1\.0

**Suggested fix:** Dependencies lack version pinning, allowing potential malicious package updates\. Consider pinning versions\. Pin all dependency versions in requirements\.txt or pyproject\.toml\. Use exact versions \(==\) or compatible ranges\. Run pip\-audit regularly\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: Unverifiable Dependency: mcp has 16 known advisory\(ies\) \(CVE\-2025\-53366 \(MCP Python SDK vulnerability in the FastMCP Server causes validation error, lead\); CVE\-2026\-116685 \(Model Context Protocol Python SDK: HTTP client transports followed cross\-origin \); CVE\-2026\-59951 \(MCP Python SDK: Unbounded Session Accumulation in StreamableHTTP Transport Enabl\) \+13 more\), but the manifest does not pin a version, so it is unknown whether the installed release is affected \(SC4\) \(low\):** Supply Chain: mcp

**File:** scripts/requirements\.txt

**Line:** 2

**Suggested fix:** Dependency has known vulnerabilities \(CVEs\)\. Using packages with unpatched security flaws exposes the environment to known exploits\. Update the dependency to a patched version that addresses the known CVE\. Check OSV \(osv\.dev\) or NVD for details on the vulnerability\.

**Finding metadata:** \{"skillspector\_confidence": 0\.4\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\) in SKILL\.md:71

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\) in SKILL\.md:93

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\) in SKILL\.md:151

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\_v2\.md \(partial\) in SKILL\.md:235

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\.md \(partial\) in SKILL\.md:72

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\.md \(partial\) in SKILL\.md:93

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: reference/node\_mcp\_server\.md \(partial\) in SKILL\.md:244

**Error:** \[SECURITY\-HIGH\] Excessive Agency: \-m, \-\-model           Claude model to use \(default: claude\-3\-7\-sonnet\-20250219\) in reference/evaluation\.md:488

**Error:** \[SECURITY\-HIGH\] Privilege Escalation: access tokens in reference/mcp\_best\_practices\.md:158

**Warning:** \[SECURITY\-MEDIUM\] MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\. in SKILL\.md:1

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub in SKILL\.md:64

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub in SKILL\.md:66

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub in reference/node\_mcp\_server\_v2\.md:712

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub in SKILL\.md:152

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub in reference/node\_mcp\_server\_v2\.md:684

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: call any tools in reference/evaluation\.md:205

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.example\.com/ in reference/node\_mcp\_server\.md:603

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.example\.com/ in reference/node\_mcp\_server\_v2\.md:294

**Warning:** \[SECURITY\-MEDIUM\] Data Exfiltration: https://api\.example\.com/ in reference/python\_mcp\_server\.md:353

**Warning:** \[SECURITY\-MEDIUM\] Excessive Agency: auto\-approve in reference/node\_mcp\_server\_v2\.md:193

**Warning:** \[SECURITY\-MEDIUM\] MCP Rug Pull: npx commands without a version suffix \(e\.g\. @​1\.0\.0\) create a rug\-pull risk if the upstream server is compromised and pub in reference/node\_mcp\_server\_v2\.md:714

**Warning:** \[SECURITY\-LOW\] Supply Chain: anthropic&gt;=0\.39\.0 in scripts/requirements\.txt:1

**Warning:** \[SECURITY\-LOW\] Supply Chain: anthropic in scripts/requirements\.txt:1

**Warning:** \[SECURITY\-LOW\] Supply Chain: mcp&gt;=1\.1\.0  in scripts/requirements\.txt:2

**Warning:** \[SECURITY\-LOW\] Supply Chain: mcp in scripts/requirements\.txt:2

**Scanner message:** skillspector risk score: 100/100 \(CRITICAL\)

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 10 files for PII

**Evidence metadata:** \{"file\_count": 10\}

**Finding: emails \(high\):** Non\-placeholder email address: john@​acme\.com

**File:** reference/node\_mcp\_server\_v2\.md

**Line:** 397

**Source line:**   \- "Look up john@​acme\.com" \-&gt; query="john@​acme\.com"

**Suggested fix:** Remove the address or use a placeholder like user@​example\.com

**Finding metadata:** \{"confidence": "high", "matched\_value": "john@​acme\.com", "occurrence\_count": 1, "occurrences": \[\{"file": "reference/node\_mcp\_server\_v2\.md", "line": 397\}\]\}

**Error:** \[PII\-HIGH\] Non\-placeholder email address: john@​acme\.com in reference/node\_mcp\_server\_v2\.md:397

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 10 files for PII

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 1: Found license declaration in frontmatter \(SKILL\.md\)

**Scanner message:**   License field references file: 'Complete terms in LICENSE\.txt'

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: semgrep:** Semgrep: No security issues found

**Finding: B314:blacklist \(medium\):** Using xml\.etree\.ElementTree\.parse to parse untrusted XML data is known to be vulnerable to XML attacks\. Replace xml\.etree\.ElementTree\.parse with its defusedxml equivalent function or make sure defusedxml\.defuse\_stdlib\(\) is called \(CWE\-20\)

**File:** /workspace/skills/mcp\-builder/scripts/evaluation\.py

**Line:** 59

**Suggested fix:** Review blacklist \(B314\) \(CWE\-20\)

**Finding metadata:** \{"cwe": 20\}

**Error:** \[BANDIT\-MEDIUM\] Using xml\.etree\.ElementTree\.parse to parse untrusted XML data is known to be vulnerable to XML attacks\. Replace xml\.etree\.ElementTree\.parse with its defusedxml equivalent function or make sure defusedxml\.defuse\_stdlib\(\) is called \(CWE\-20\) in /workspace/skills/mcp\-builder/scripts/evaluation\.py:59

**Scanner message:** Found 2 Python, 0 Shell, 0 JavaScript/TypeScript files

**Scanner message:** Bandit found: 0 HIGH, 1 MEDIUM, 0 LOW

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 6 markdown files for dead links

**Evidence metadata:** \{"file\_count": 6\}

**Evidence: dead\_links:** All relative links valid in 6 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 6\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 6 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 6 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 10 file\(s\)

**Evidence metadata:** \{"files\_scanned": 10\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 10 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 81\.5/100 \(Grade: B\)

**Evidence metadata:** \{"grade": "B", "overall\_score": 81\.5, "skill\_type": "script\-based"\}

**Finding: quality\_correctness \(medium\):** No documented scripts in table format

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add '\#\# Available Scripts' with table: \| Script \| Purpose \| Arguments \|

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** Instructions don't mention 'run\_script'

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add explicit run\_script\(\) call examples

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(277 chars, recommend 50\-150\)

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/mcp\-builder/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Warning:** \[QUALITY\-MEDIUM\] No documented scripts in table format in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Instructions don't mention 'run\_script' in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(277 chars, recommend 50\-150\) in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/mcp\-builder/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/mcp\-builder/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 81\.5/100 \(Grade: B\)

### SCRIPT\_LINT — evidence

**Finding: magic\_numbers \(low\):** connections\.py contains magic numbers

**File:** /workspace/skills/mcp\-builder/scripts/connections\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** connections\.py missing shebang line

**File:** /workspace/skills/mcp\-builder/scripts/connections\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** evaluation\.py contains magic numbers

**File:** /workspace/skills/mcp\-builder/scripts/evaluation\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** evaluation\.py missing shebang line

**File:** /workspace/skills/mcp\-builder/scripts/evaluation\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Warning:** \[SCRIPT\_LINT\-LOW\] connections\.py contains magic numbers in /workspace/skills/mcp\-builder/scripts/connections\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] connections\.py missing shebang line in /workspace/skills/mcp\-builder/scripts/connections\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] evaluation\.py contains magic numbers in /workspace/skills/mcp\-builder/scripts/evaluation\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] evaluation\.py missing shebang line in /workspace/skills/mcp\-builder/scripts/evaluation\.py

## skills/pdf

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-014) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-014/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-014/skillevaluator-tier1.json)

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

**Finding: unexpected\_file \(low\):** Unexpected 'forms\.md' in skill root

**File:** /workspace/skills/pdf/forms\.md

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'reference\.md' in skill root

**File:** /workspace/skills/pdf/reference\.md

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

**Warning:** \[SCHEMA\-LOW\] Unexpected 'forms\.md' in skill root in /workspace/skills/pdf/forms\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'reference\.md' in skill root in /workspace/skills/pdf/reference\.md

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

## skills/pptx

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-015) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-015/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-015/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 75 | 0\.35 | 4 |
| discoverability | 75 | 0\.25 | 4 |
| reliability | 80 | 0\.25 | 4 |
| efficiency | 85 | 0\.15 | 1 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 8 | 1 | 4 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 7 | 19 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | FAIL | 0 | 1 | 0 |
| Code Risk Analysis | PASS | 2 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 13 |
| SCRIPT\_LINT | PASS | 0 | 0 | 8 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/pptx/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'pptx'

**Evidence metadata:** \{"description\_length": 732\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/pptx/

**Evidence: naming\_convention:** Folder name 'pptx' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 4\}

**Evidence: line\_count:** SKILL\.md within line limit \(238/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 238\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: optional\_files:** Found optional supporting files: scripts

**Evidence metadata:** \{"files\_found": \["scripts"\]\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'pptx'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/pptx/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/pptx/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/pptx/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'pptx'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/pptx/

**Scanner message:** \[OK\] naming\_convention: Folder name 'pptx' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(238/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] optional\_files: Found optional supporting files: scripts

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'pptx'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Tool Parameter Abuse \(TM1\) \(high\):** Tool Misuse: rm \-f \.\./out\.pptx

**File:** SKILL\.md

**Line:** 62

**Source line:** \# reorder / delete slides = edit &lt;p:sldIdLst&gt; in ppt/presentation\.xml python scripts/clean\.py unpacked/                                     \# after deletions: removes orphaned slides, media, rels \# ed

**Suggested fix:** Tool parameters are crafted to achieve unintended or unsafe behavior\. Parameter abuse can bypass intended safety checks \(e\.g\. shell=True, \-\-force, dangerous glob patterns\)\. Validate all tool parameters against an allowlist\. Reject dangerous parameter values \(shell=True, \-\-force, \-rf /\) and use safe defaults\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Chaining Abuse \(TM2\) \(high\):** Tool Misuse: &amp;&amp; rm \-

**File:** SKILL\.md

**Line:** 62

**Source line:** \# reorder / delete slides = edit &lt;p:sldIdLst&gt; in ppt/presentation\.xml python scripts/clean\.py unpacked/                                     \# after deletions: removes orphaned slides, media, rels \# ed

**Suggested fix:** Tool calls are chained to bypass individual safety checks or escalate capabilities beyond what any single tool call would allow\. Limit tool chaining depth and validate the output of each tool before passing it to the next\. Require explicit user approval for multi\-step chains\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Hidden Instructions \(P2\) \(high\):** Prompt Injection: ﻿

**File:** scripts/office/schemas/ecma/fouth\-edition/opc\-contentTypes\.xsd

**Line:** 1

**Source line:** ﻿&lt;?xml version="1\.0" encoding="UTF\-8" standalone="no"?&gt; &lt;xs:schema xmlns="http://schemas\.openxmlformats\.org/package/2006/content\-types"   xmlns:xs="http://www\.w3\.org/2001/XMLSchema"   targetNamespace=

**Suggested fix:** Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Hidden Instructions \(P2\) \(high\):** Prompt Injection: ﻿

**File:** scripts/office/schemas/ecma/fouth\-edition/opc\-coreProperties\.xsd

**Line:** 1

**Source line:** ﻿&lt;?xml version="1\.0" encoding="UTF\-8"?&gt; &lt;xs:schema targetNamespace="http://schemas\.openxmlformats\.org/package/2006/metadata/core\-properties"   xmlns="http://schemas\.openxmlformats\.org/package/2006/met

**Suggested fix:** Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Hidden Instructions \(P2\) \(high\):** Prompt Injection: ﻿

**File:** scripts/office/schemas/ecma/fouth\-edition/opc\-relationships\.xsd

**Line:** 1

**Source line:** ﻿&lt;?xml version="1\.0" encoding="UTF\-8" standalone="no"?&gt; &lt;xsd:schema xmlns="http://schemas\.openxmlformats\.org/package/2006/relationships"   xmlns:xsd="http://www\.w3\.org/2001/XMLSchema"   targetNamespac

**Suggested fix:** Hidden instructions were detected in comments or invisible text\. These could contain malicious directives\. Manual review is recommended\. Audit all comments and invisible characters\. Remove any instructions that direct the agent to perform unauthorized actions\. Use plain, reviewable content\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Env Variable Harvesting \(E2\) \(high\):** Data Exfiltration: os\.environ\.copy\(\)

**File:** scripts/office/soffice\.py

**Line:** 28

**Source line:**   def get\_soffice\_env\(\) \-&gt; dict:     env = os\.environ\.copy\(\)     env\["SAL\_USE\_VCLPLUGIN"\] = "svp"      if \_needs\_shim\(\):

**Suggested fix:** Code enumerates, copies, or searches environment variables for secrets\. Bulk environment access can collect credentials unrelated to the skill's stated purpose\. Read only explicitly required environment variables by name\. Avoid enumerating or copying the full environment, and never log or transmit credentials to untrusted destinations\.

**Finding metadata:** \{"skillspector\_confidence": 0\.6\}

**Finding: Unknown \(LP3\) \(medium\):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Unsafe Defaults \(TM3\) \(medium\):** Tool Misuse: mode = 0o666

**File:** scripts/office/helpers/\_\_init\_\_\.py

**Line:** 106

**Source line:**         else:             umask = os\.umask\(0\)             os\.umask\(umask\)             mode = 0o666 &amp; \~umask         os\.chmod\(tmp\_out, mode\)         os\.replace\(tmp\_out, out\_path\)     finally:

**Suggested fix:** Tool defaults are unsafe or overly permissive \(e\.g\. disabled TLS verification, no authentication, world\-writable permissions\)\. Unsafe defaults widen the attack surface\. Override unsafe defaults with secure settings \(verify=True, auth required, restrictive permissions\)\. Review and harden all tool configurations\.

**Finding metadata:** \{"skillspector\_confidence": 0\.8\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 1455

**Source line:**     &lt;/xsd:sequence&gt;     &lt;xsd:attribute name="pos" type="ST\_PositiveFixedPercentage" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_GradientStopList"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:e

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 1462

**Source line:**   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_GradientFillProperties"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:element name="gsLst" type="CT\_GradientStopList" minOccurs="0" maxOccurs="1"/&gt;       &lt;xsd:group r

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 2189

**Source line:**     &lt;xsd:attribute name="d" type="ST\_PositivePercentage" use="required"/&gt;     &lt;xsd:attribute name="sp" type="ST\_PositivePercentage" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_Da

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 2197

**Source line:**   &lt;xsd:group name="EG\_LineDashProperties"&gt;     &lt;xsd:choice&gt;       &lt;xsd:element name="prstDash" type="CT\_PresetLineDashProperties" minOccurs="1" maxOccurs="1"/&gt;       &lt;xsd:element name="custDash" type=

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 2992

**Source line:**     &lt;xsd:attribute name="pos" type="ST\_Coordinate32" use="optional"/&gt;     &lt;xsd:attribute name="algn" type="ST\_TextTabAlignType" use="optional"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_TextTa

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd

**Line:** 3043

**Source line:**       &lt;xsd:group ref="EG\_TextBulletSize" minOccurs="0" maxOccurs="1"/&gt;       &lt;xsd:group ref="EG\_TextBulletTypeface" minOccurs="0" maxOccurs="1"/&gt;       &lt;xsd:group ref="EG\_TextBullet" minOccurs="0" max

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 730

**Source line:**     &lt;xsd:attribute name="st" type="ST\_Index" use="required"/&gt;     &lt;xsd:attribute name="end" type="ST\_Index" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_SlideRelationshipListEntry

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 733

**Source line:**   &lt;xsd:complexType name="CT\_SlideRelationshipListEntry"&gt;     &lt;xsd:attribute ref="r:id" use="required"/&gt;   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_SlideRelationshipList"&gt;     &lt;xsd:sequence&gt;     

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 735

**Source line:**   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_SlideRelationshipList"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:element name="sld" type="CT\_SlideRelationshipListEntry" minOccurs="0"         maxOccurs="unbounde

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd

**Line:** 950

**Source line:**   &lt;/xsd:complexType&gt;   &lt;xsd:complexType name="CT\_CustomShow"&gt;     &lt;xsd:sequence&gt;       &lt;xsd:element name="sldLst" type="CT\_SlideRelationshipList" minOccurs="1" maxOccurs="1"/&gt;       &lt;xsd:element name=

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/microsoft/wml\-2010\.xsd

**Line:** 181

**Source line:**      &lt;/xsd:sequence&gt;      &lt;xsd:attribute name="pos" type="a:ST\_PositiveFixedPercentage" use="required"/&gt;    &lt;/xsd:complexType&gt;    &lt;xsd:complexType name="CT\_GradientStopList"&gt;      &lt;xsd:sequence&gt;      

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: pList

**File:** scripts/office/schemas/microsoft/wml\-2010\.xsd

**Line:** 209

**Source line:**    &lt;/xsd:complexType&gt;    &lt;xsd:complexType name="CT\_GradientFillProperties"&gt;      &lt;xsd:sequence&gt;        &lt;xsd:element name="gsLst" type="CT\_GradientStopList" minOccurs="0"/&gt;        &lt;xsd:group ref="EG\_Sh

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.75\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(\["soffice"\] \+ args, env=get\_soffice\_env\(\), \*\*kwargs\)

**File:** scripts/office/soffice\.py

**Line:** 46

**Source line:**                 tempfile\.TemporaryDirectory\(prefix="lo\_profile\_", ignore\_cleanup\_errors=True\)             \)             args = \[f"\-env:UserInstallation=\{Path\(profile\)\.as\_uri\(\)\}"\] \+ args         return

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(         \["gcc", "\-shared", "\-fPIC", "\-o", str\(\_SHIM\_SO\), str\(src\), "\-ldl"\],         check=True,         capture\_output=True,     \)

**File:** scripts/office/soffice\.py

**Line:** 68

**Source line:**      src = Path\(tempfile\.gettempdir\(\)\) / "lo\_socket\_shim\.c"     src\.write\_text\(\_SHIM\_SOURCE\)     subprocess\.run\(         \["gcc", "\-shared", "\-fPIC", "\-o", str\(\_SHIM\_SO\), str\(src\), "\-ldl"\],         che

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-\-word\-diff\-regex=\.",        

**File:** scripts/office/validators/redlining\.py

**Line:** 192

**Source line:**                 original\_file\.write\_text\(original\_text, encoding="utf\-8"\)                 modified\_file\.write\_text\(modified\_text, encoding="utf\-8"\)                  result = subprocess\.run\(           

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-U0",                        

**File:** scripts/office/validators/redlining\.py

**Line:** 221

**Source line:**                     if content\_lines:                         return "\\n"\.join\(content\_lines\)                  result = subprocess\.run\(                     \[                         "git",            

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(         \[             "pdftoppm",             "\-jpeg",             "\-r",             str\(CONVERSION\_DPI\),             str\(pdf\_path\),             str\(temp\_dir / "slide"\),         \],    

**File:** scripts/thumbnail\.py

**Line:** 200

**Source line:**         detail = \(result\.stderr or result\.stdout or ""\)\.strip\(\)         raise RuntimeError\(f"PDF conversion failed: \{detail\}" if detail else "PDF conversion failed"\)      result = subprocess\.run\(     

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Error:** \[SECURITY\-HIGH\] Tool Misuse: rm \-f \.\./out\.pptx in SKILL\.md:62

**Error:** \[SECURITY\-HIGH\] Tool Misuse: &amp;&amp; rm \- in SKILL\.md:62

**Error:** \[SECURITY\-HIGH\] Prompt Injection: ﻿ in scripts/office/schemas/ecma/fouth\-edition/opc\-contentTypes\.xsd:1

**Error:** \[SECURITY\-HIGH\] Prompt Injection: ﻿ in scripts/office/schemas/ecma/fouth\-edition/opc\-coreProperties\.xsd:1

**Error:** \[SECURITY\-HIGH\] Prompt Injection: ﻿ in scripts/office/schemas/ecma/fouth\-edition/opc\-relationships\.xsd:1

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: os\.environ\.copy\(\) in scripts/office/soffice\.py:28

**Warning:** \[SECURITY\-MEDIUM\] MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\. in SKILL\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Tool Misuse: mode = 0o666 in scripts/office/helpers/\_\_init\_\_\.py:106

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:1455

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:1462

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:2189

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:2197

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:2992

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/dml\-main\.xsd:3043

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:730

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:733

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:735

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/ISO\-IEC29500\-4\_2016/pml\.xsd:950

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/microsoft/wml\-2010\.xsd:181

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: pList in scripts/office/schemas/microsoft/wml\-2010\.xsd:209

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(\["soffice"\] \+ args, env=get\_soffice\_env\(\), \*\*kwargs\) in scripts/office/soffice\.py:46

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(         \["gcc", "\-shared", "\-fPIC", "\-o", str\(\_SHIM\_SO\), str\(src\), "\-ldl"\],         check=True,         capture\_output=True,     \) in scripts/office/soffice\.py:68

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-\-word\-diff\-regex=\.",         in scripts/office/validators/redlining\.py:192

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(                     \[                         "git",                         "diff",                         "\-\-word\-diff=plain",                         "\-U0",                         in scripts/office/validators/redlining\.py:221

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(         \[             "pdftoppm",             "\-jpeg",             "\-r",             str\(CONVERSION\_DPI\),             str\(pdf\_path\),             str\(temp\_dir / "slide"\),         \],     in scripts/thumbnail\.py:200

**Scanner message:** skillspector risk score: 100/100 \(CRITICAL\)

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 17 files for PII

**Evidence metadata:** \{"file\_count": 17\}

**Evidence: pii\_detection:** No PII detected in 17 files \(emails, SSNs, phone numbers, paths\)

**Evidence metadata:** \{"files\_scanned": 17\}

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 17 files for PII

**Scanner message:** \[OK\] pii\_detection: No PII detected in 17 files \(emails, SSNs, phone numbers, paths\)

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

**Scanner message:** Found 15 Python, 0 Shell, 0 JavaScript/TypeScript files

**Scanner message:** \[OK\] bandit: Bandit: No security issues found

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 1 markdown files for dead links

**Evidence metadata:** \{"file\_count": 1\}

**Evidence: dead\_links:** All relative links valid in 1 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 1\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 1 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 1 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 17 file\(s\)

**Evidence metadata:** \{"files\_scanned": 17\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 17 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 77\.8/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 77\.8, "skill\_type": "script\-based"\}

**Finding: quality\_correctness \(medium\):** Instructions don't mention 'run\_script'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add explicit run\_script\(\) call examples

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(732 chars, recommend 50\-150\)

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** Broad description without negative triggers may cause over\-triggering

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add boundary phrases like 'Do NOT use for\.\.\.'

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(medium\):** Skill name very short: 'pptx'

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Use descriptive names like 'crypto\-utils' not 'crypto'

**Finding metadata:** \{"deduction": 10, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** Scripts may lack error handling: \_\_init\_\_\.py

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Scripts should handle errors explicitly

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_efficiency \(medium\):** Large skill \(5161 tokens, recommended max &lt;5000\)\. Per agentskills\.io, SKILL\.md should be concise \(\~500 lines\) — large skill bodies increase token cost after invocation; long or unfocused top\-level descriptions can degrade agent routing accuracy

**File:** /workspace/skills/pptx/SKILL\.md

**Suggested fix:** Keep required sections concise; move detailed examples, reference material, and supporting docs to the references/ directory

**Finding metadata:** \{"deduction": 15, "dimension": "efficiency"\}

**Warning:** \[QUALITY\-MEDIUM\] Instructions don't mention 'run\_script' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(732 chars, recommend 50\-150\) in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Broad description without negative triggers may cause over\-triggering in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Skill name very short: 'pptx' in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Scripts may lack error handling: \_\_init\_\_\.py in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/pptx/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Large skill \(5161 tokens, recommended max &lt;5000\)\. Per agentskills\.io, SKILL\.md should be concise \(\~500 lines\) — large skill bodies increase token cost after invocation; long or unfocused top\-level descriptions can degrade agent routing accuracy in /workspace/skills/pptx/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 77\.8/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Finding: flat\_script \(medium\):** \_\_init\_\_\.py has no function definitions \(flat script\)

**File:** /workspace/skills/pptx/scripts/\_\_init\_\_\.py

**Suggested fix:** Wrap logic in functions for maintainability and testability

**Finding: missing\_shebang \(low\):** \_\_init\_\_\.py missing shebang line

**File:** /workspace/skills/pptx/scripts/\_\_init\_\_\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: no\_input\_validation \(low\):** \_\_init\_\_\.py may lack input validation

**File:** /workspace/skills/pptx/scripts/\_\_init\_\_\.py

**Suggested fix:** Add argument checks and raise descriptive errors

**Finding: magic\_numbers \(low\):** add\_slide\.py contains magic numbers

**File:** /workspace/skills/pptx/scripts/add\_slide\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** add\_slide\.py missing shebang line

**File:** /workspace/skills/pptx/scripts/add\_slide\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: missing\_shebang \(low\):** clean\.py missing shebang line

**File:** /workspace/skills/pptx/scripts/clean\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: magic\_numbers \(low\):** thumbnail\.py contains magic numbers

**File:** /workspace/skills/pptx/scripts/thumbnail\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** thumbnail\.py missing shebang line

**File:** /workspace/skills/pptx/scripts/thumbnail\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Warning:** \[SCRIPT\_LINT\-MEDIUM\] \_\_init\_\_\.py has no function definitions \(flat script\) in /workspace/skills/pptx/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] \_\_init\_\_\.py missing shebang line in /workspace/skills/pptx/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] \_\_init\_\_\.py may lack input validation in /workspace/skills/pptx/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] add\_slide\.py contains magic numbers in /workspace/skills/pptx/scripts/add\_slide\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] add\_slide\.py missing shebang line in /workspace/skills/pptx/scripts/add\_slide\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] clean\.py missing shebang line in /workspace/skills/pptx/scripts/clean\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] thumbnail\.py contains magic numbers in /workspace/skills/pptx/scripts/thumbnail\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] thumbnail\.py missing shebang line in /workspace/skills/pptx/scripts/thumbnail\.py

## skills/skill\-creator

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-016) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-016/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-016/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 65 | 0\.35 | 5 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 80 | 0\.25 | 4 |
| efficiency | 80 | 0\.15 | 2 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 8 | 1 | 5 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 5 | 5 |
| PII Scan | PASS | 1 | 0 | 1 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | PASS | 2 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 4 | 0 | 1 |
| Dependency Vulnerability Audit | NOT APPLICABLE | 1 | 0 | 0 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 13 |
| SCRIPT\_LINT | PASS | 0 | 0 | 11 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/skill\-creator/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'skill\-creator'

**Evidence metadata:** \{"description\_length": 319\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/skill\-creator/

**Evidence: naming\_convention:** Folder name 'skill\-creator' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 13\}

**Evidence: line\_count:** SKILL\.md within line limit \(485/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 485\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: optional\_files:** Found optional supporting files: agents, assets, references, scripts

**Evidence metadata:** \{"files\_found": \["agents", "assets", "references", "scripts"\]\}

**Evidence: name\_consistency:** Directory name matches frontmatter: 'skill\-creator'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/skill\-creator/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'eval\-viewer' in skill root

**File:** /workspace/skills/skill\-creator/eval\-viewer

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/skill\-creator/LICENSE\.txt

**Warning:** \[SCHEMA\-LOW\] Unexpected 'eval\-viewer' in skill root in /workspace/skills/skill\-creator/eval\-viewer

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'skill\-creator'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/skill\-creator/

**Scanner message:** \[OK\] naming\_convention: Folder name 'skill\-creator' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(485/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] optional\_files: Found optional supporting files: agents, assets, references, scripts

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'skill\-creator'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Incomplete referenced artifact analysis \(AE1\) \(high\):** analysis\-evasion: assets/eval\_review\.html \(partial\)

**File:** SKILL\.md

**Line:** 364

**Source line:** 1\. Read the template from \`assets/eval\_review\.html\`

**Suggested fix:** Referenced artifact was not completely inspected Review the reported expression and analyzer's parsing limitation; correct the scanner if it misinterprets valid source, then rerun the scan\. Keep required references; incomplete analysis is not proof of malicious evasion\.

**Finding metadata:** \{"skillspector\_confidence": 1\.0\}

**Finding: Env Variable Harvesting \(E2\) \(high\):** Data Exfiltration: os\.environ\.items\(\)

**File:** scripts/improve\_description\.py

**Line:** 33

**Source line:**     \# Remove CLAUDECODE env var to allow nesting claude \-p inside a     \# Claude Code session\. The guard is for interactive terminal conflicts;     \# programmatic subprocess usage is safe\. Same patter

**Suggested fix:** Code enumerates, copies, or searches environment variables for secrets\. Bulk environment access can collect credentials unrelated to the skill's stated purpose\. Read only explicitly required environment variables by name\. Avoid enumerating or copying the full environment, and never log or transmit credentials to untrusted destinations\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Env Variable Harvesting \(E2\) \(high\):** Data Exfiltration: os\.environ\.items\(\)

**File:** scripts/run\_eval\.py

**Line:** 83

**Source line:**         \# Remove CLAUDECODE env var to allow nesting claude \-p inside a         \# Claude Code session\. The guard is for interactive terminal conflicts;         \# programmatic subprocess usage is safe\.

**Suggested fix:** Code enumerates, copies, or searches environment variables for secrets\. Bulk environment access can collect credentials unrelated to the skill's stated purpose\. Read only explicitly required environment variables by name\. Avoid enumerating or copying the full environment, and never log or transmit credentials to untrusted destinations\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Agent Config Directory Access \(AS1\) \(high\):** Agent Snooping: Find the project root by walking up from cwd looking for \.claude/

**File:** scripts/run\_eval\.py

**Line:** 23

**Source line:**   def find\_project\_root\(\) \-&gt; Path:     """Find the project root by walking up from cwd looking for \.claude/\.      Mimics how Claude Code discovers its project root, so the command file     we create e

**Suggested fix:** Skill reads from agent configuration directories \(\.claude/, \.codex/, \.gemini/\)\. These directories may contain API keys, personal settings, and other credentials that the skill has no legitimate need to access\. Remove all code or instructions that access agent configuration directories \(\.claude/, \.codex/, \.gemini/\)\. If configuration values are needed, pass them explicitly as parameters or environment variables — never read the agent's own config files\.

**Finding metadata:** \{"skillspector\_confidence": 0\.85\}

**Finding: Unknown \(LP3\) \(medium\):** MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\.

**File:** SKILL\.md

**Line:** 1

**Suggested fix:** Without declared permissions the skill's intent is opaque and cannot be validated\. Declare the skill's tool scope: for Claude Code / Agent Skills SKILL\.md, list the tools the skill may invoke in the 'allowed\-tools' frontmatter field; for MCP server manifests, add a 'permissions' list naming the required capabilities\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: Session Persistence \(RA2\) \(medium\):** Rogue Agent: nohup 

**File:** SKILL\.md

**Line:** 238

**Source line:**  4\. \*\*Launch the viewer\*\* with both qualitative outputs and quantitative data:    \`\`\`bash    nohup python &lt;skill\-creator\-path&gt;/eval\-viewer/generate\_review\.py \\      &lt;workspace&gt;/iteration\-N \\      \-\-sk

**Suggested fix:** Skill establishes unauthorized persistence across sessions via cron jobs, startup scripts, or state files\. Session persistence allows an attacker to maintain access beyond the current interaction\. Remove any persistence mechanisms \(cron jobs, startup scripts, state files\)\. Skills should not maintain state across sessions without explicit user consent\.

**Finding metadata:** \{"skillspector\_confidence": 0\.65\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(             \["lsof", "\-ti", f":\{port\}"\],             capture\_output=True, text=True, timeout=5,         \)

**File:** eval\-viewer/generate\_review\.py

**Line:** 291

**Source line:** def \_kill\_port\(port: int\) \-&gt; None:     """Kill any process listening on the given port\."""     try:         result = subprocess\.run\(             \["lsof", "\-ti", f":\{port\}"\],             capture\_output

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.run\(         cmd,         input=prompt,         capture\_output=True,         text=True,         env=env,         timeout=timeout,     \)

**File:** scripts/improve\_description\.py

**Line:** 35

**Source line:**     \# programmatic subprocess usage is safe\. Same pattern as run\_eval\.py\.     env = \{k: v for k, v in os\.environ\.items\(\) if k \!= "CLAUDECODE"\}      result = subprocess\.run\(         cmd,         input=

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Finding: subprocess module call \(AST4\) \(medium\):** Dangerous Code Execution: subprocess\.Popen\(             cmd,             stdout=subprocess\.PIPE,             stderr=subprocess\.DEVNULL,             cwd=project\_root,             env=env,         \)

**File:** scripts/run\_eval\.py

**Line:** 85

**Source line:**         \# programmatic subprocess usage is safe\.         env = \{k: v for k, v in os\.environ\.items\(\) if k \!= "CLAUDECODE"\}          process = subprocess\.Popen\(             cmd,             stdout=subpr

**Suggested fix:** subprocess module calls execute external commands\. Without careful input validation, this enables command injection\. Use subprocess\.run\(\) with shell=False and an explicit argument list\. Validate all inputs and avoid passing user\-controlled data to commands\.

**Finding metadata:** \{"skillspector\_confidence": 0\.7\}

**Error:** skillspector JSON field 'analysis\_completeness' reports incomplete analysis \(status 'partial'\); security scan did not complete

**Error:** \[SECURITY\-HIGH\] analysis\-evasion: assets/eval\_review\.html \(partial\) in SKILL\.md:364

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: os\.environ\.items\(\) in scripts/improve\_description\.py:33

**Error:** \[SECURITY\-HIGH\] Data Exfiltration: os\.environ\.items\(\) in scripts/run\_eval\.py:83

**Error:** \[SECURITY\-HIGH\] Agent Snooping: Find the project root by walking up from cwd looking for \.claude/ in scripts/run\_eval\.py:23

**Warning:** \[SECURITY\-MEDIUM\] MCP Least Privilege: Without declared permissions the skill's intent is opaque and cannot be validated\. in SKILL\.md:1

**Warning:** \[SECURITY\-MEDIUM\] Rogue Agent: nohup  in SKILL\.md:238

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(             \["lsof", "\-ti", f":\{port\}"\],             capture\_output=True, text=True, timeout=5,         \) in eval\-viewer/generate\_review\.py:291

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.run\(         cmd,         input=prompt,         capture\_output=True,         text=True,         env=env,         timeout=timeout,     \) in scripts/improve\_description\.py:35

**Warning:** \[SECURITY\-MEDIUM\] Dangerous Code Execution: subprocess\.Popen\(             cmd,             stdout=subprocess\.PIPE,             stderr=subprocess\.DEVNULL,             cwd=project\_root,             env=env,         \) in scripts/run\_eval\.py:85

**Scanner message:** skillspector risk score: 100/100 \(CRITICAL\)

**Incomplete scanners:** \["skillspector"\]

### PII Scan — evidence

**Evidence: pii\_scan\_start:** Scanning 16 files for PII

**Evidence metadata:** \{"file\_count": 16\}

**Finding: phone\_numbers \(medium\):** International phone number: \+1700 — 2 occurrences \(references/schemas\.md lines 275, 302\)

**File:** references/schemas\.md

**Line:** 275

**Source line:**       "tokens": "\+1700"

**Suggested fix:** Remove phone number or use placeholder like \+1\-555\-555\-5555

**Finding metadata:** \{"confidence": "high", "matched\_value": "\+1700", "occurrence\_count": 2, "occurrences": \[\{"file": "references/schemas\.md", "line": 275\}, \{"file": "references/schemas\.md", "line": 302\}\]\}

**Warning:** \[PII\-MEDIUM\] International phone number: \+1700 — 2 occurrences \(references/schemas\.md lines 275, 302\) in references/schemas\.md:275

**Scanner message:** \[OK\] pii\_scan\_start: Scanning 16 files for PII

### License Compliance — evidence

**Evidence: license\_compliance:** License compliance scan completed \(allowed\)

**Evidence metadata:** \{"license\_status": "allowed"\}

**Scanner message:** Tier 2: Detected Apache\-2\.0 from LICENSE\.txt

**Scanner message:** License: Apache\-2\.0 \(ALLOWED \- permissive\)

**Scanner message:** \[OK\] license\_compliance: License compliance scan completed \(allowed\)

### Code Risk Analysis — evidence

**Evidence: bandit:** Bandit: No security issues found

**Evidence: semgrep:** Semgrep: No security issues found

**Scanner message:** Found 10 Python, 0 Shell, 0 JavaScript/TypeScript files

**Scanner message:** \[OK\] bandit: Bandit: No security issues found

**Scanner message:** \[OK\] semgrep: Semgrep: No security issues found

### Secrets Detection — evidence

**Evidence: gitleaks:** No secrets detected by Gitleaks

**Scanner message:** \[OK\] gitleaks: No secrets detected by Gitleaks

### Code Integrity &amp; Hygiene — evidence

**Evidence: dead\_links\_scan:** Checking 5 markdown files for dead links

**Evidence metadata:** \{"file\_count": 5\}

**Evidence: dead\_links:** All relative links valid in 5 markdown file\(s\)

**Evidence metadata:** \{"files\_checked": 5\}

**Evidence: dependencies:** No dependency files found \(requirements\.txt, pyproject\.toml\)

**Evidence: test\_discovery:** No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

**Evidence metadata:** \{"coverage\_measured": false, "execution\_performed": false, "patterns": \["test\_\*\.py", "\*\_test\.py"\], "test\_count": 0\}

**Warning:** No standard Python test\-file candidates found; consider adding tests

**Scanner message:** \[OK\] dead\_links\_scan: Checking 5 markdown files for dead links

**Scanner message:** \[OK\] dead\_links: All relative links valid in 5 markdown file\(s\)

**Scanner message:** \[OK\] dependencies: No dependency files found \(requirements\.txt, pyproject\.toml\)

**Scanner message:** \[OK\] test\_discovery: No standard Python test\-file candidates found; target tests were not executed and coverage was not measured\. Consider adding tests\.

### Dependency Vulnerability Audit — evidence

**Evidence: dependency\_file\_discovery:** No dependency files found \- vulnerability audit is not applicable

**Scanner message:** \[OK\] dependency\_file\_discovery: No dependency files found \- vulnerability audit is not applicable

### Unicode Smuggling Detection — evidence

**Evidence: unicode\_scan:** No invisible Unicode characters detected in 18 file\(s\)

**Evidence metadata:** \{"files\_scanned": 18\}

**Scanner message:** \[OK\] unicode\_scan: No invisible Unicode characters detected in 18 file\(s\)

### QUALITY — evidence

**Evidence: quality\_score:** Score: 77\.2/100 \(Grade: C\)

**Evidence metadata:** \{"grade": "C", "overall\_score": 77\.2, "skill\_type": "hybrid"\}

**Finding: quality\_correctness \(medium\):** No documented scripts in table format

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add '\#\# Available Scripts' with table: \| Script \| Purpose \| Arguments \|

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** Instructions don't mention 'run\_script'

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add explicit run\_script\(\) call examples

**Finding metadata:** \{"deduction": 10, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'version'

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add 'version' to frontmatter — Semantic version \(e\.g\., "1\.0\.0"\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.author'

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add 'author' under metadata: — Author name or team \(under metadata:\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_correctness \(medium\):** SKILL\_SPEC recommended field missing: 'metadata\.tags'

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add 'tags' under metadata: — Categorization tags \(under metadata:, list of 1\-5 items\)

**Finding metadata:** \{"deduction": 5, "dimension": "correctness"\}

**Finding: quality\_discoverability \(low\):** Description very long \(319 chars, recommend 50\-150\)

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Keep descriptions concise for progressive disclosure

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_discoverability \(low\):** No '\#\# Purpose' section

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add purpose section to clarify use cases

**Finding metadata:** \{"deduction": 5, "dimension": "discoverability"\}

**Finding: quality\_reliability \(low\):** Scripts may lack error handling: \_\_init\_\_\.py, generate\_report\.py

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Scripts should handle errors explicitly

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No prerequisites/requirements documented

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Document dependencies, API keys, or setup needed

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No limitations documented

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add '\#\# Limitations' section with known issues/constraints

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_reliability \(low\):** No troubleshooting section documented

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Add '\#\# Troubleshooting' with Error/Cause/Solution patterns

**Finding metadata:** \{"deduction": 5, "dimension": "reliability"\}

**Finding: quality\_efficiency \(medium\):** Large skill \(8246 tokens, recommended max &lt;5000\)\. Per agentskills\.io, SKILL\.md should be concise \(\~500 lines\) — large skill bodies increase token cost after invocation; long or unfocused top\-level descriptions can degrade agent routing accuracy

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Keep required sections concise; move detailed examples, reference material, and supporting docs to the references/ directory

**Finding metadata:** \{"deduction": 15, "dimension": "efficiency"\}

**Finding: quality\_efficiency \(low\):** Uses complex/corporate language

**File:** /workspace/skills/skill\-creator/SKILL\.md

**Suggested fix:** Use simple, direct language: 'use' not 'utilize'

**Finding metadata:** \{"deduction": 5, "dimension": "efficiency"\}

**Warning:** \[QUALITY\-MEDIUM\] No documented scripts in table format in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Instructions don't mention 'run\_script' in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'version' in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.author' in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] SKILL\_SPEC recommended field missing: 'metadata\.tags' in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Description very long \(319 chars, recommend 50\-150\) in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No '\#\# Purpose' section in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Scripts may lack error handling: \_\_init\_\_\.py, generate\_report\.py in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No prerequisites/requirements documented in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No limitations documented in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] No troubleshooting section documented in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-MEDIUM\] Large skill \(8246 tokens, recommended max &lt;5000\)\. Per agentskills\.io, SKILL\.md should be concise \(\~500 lines\) — large skill bodies increase token cost after invocation; long or unfocused top\-level descriptions can degrade agent routing accuracy in /workspace/skills/skill\-creator/SKILL\.md

**Warning:** \[QUALITY\-LOW\] Uses complex/corporate language in /workspace/skills/skill\-creator/SKILL\.md

**Scanner message:** \[OK\] quality\_score: Score: 77\.2/100 \(Grade: C\)

### SCRIPT\_LINT — evidence

**Finding: flat\_script \(medium\):** \_\_init\_\_\.py has no function definitions \(flat script\)

**File:** /workspace/skills/skill\-creator/scripts/\_\_init\_\_\.py

**Suggested fix:** Wrap logic in functions for maintainability and testability

**Finding: missing\_shebang \(low\):** \_\_init\_\_\.py missing shebang line

**File:** /workspace/skills/skill\-creator/scripts/\_\_init\_\_\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Finding: no\_input\_validation \(low\):** \_\_init\_\_\.py may lack input validation

**File:** /workspace/skills/skill\-creator/scripts/\_\_init\_\_\.py

**Suggested fix:** Add argument checks and raise descriptive errors

**Finding: magic\_numbers \(low\):** aggregate\_benchmark\.py contains magic numbers

**File:** /workspace/skills/skill\-creator/scripts/aggregate\_benchmark\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: magic\_numbers \(low\):** generate\_report\.py contains magic numbers

**File:** /workspace/skills/skill\-creator/scripts/generate\_report\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: magic\_numbers \(low\):** improve\_description\.py contains magic numbers

**File:** /workspace/skills/skill\-creator/scripts/improve\_description\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: magic\_numbers \(low\):** quick\_validate\.py contains magic numbers

**File:** /workspace/skills/skill\-creator/scripts/quick\_validate\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: deep\_nesting \(medium\):** run\_eval\.py has deeply nested code \(depth 9, max 6\)

**File:** /workspace/skills/skill\-creator/scripts/run\_eval\.py

**Suggested fix:** Refactor into smaller functions to reduce complexity

**Finding: magic\_numbers \(low\):** run\_eval\.py contains magic numbers

**File:** /workspace/skills/skill\-creator/scripts/run\_eval\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: magic\_numbers \(low\):** run\_loop\.py contains magic numbers

**File:** /workspace/skills/skill\-creator/scripts/run\_loop\.py

**Suggested fix:** Extract magic numbers to named constants

**Finding: missing\_shebang \(low\):** utils\.py missing shebang line

**File:** /workspace/skills/skill\-creator/scripts/utils\.py

**Suggested fix:** Add: \#\!/usr/bin/env python3

**Warning:** \[SCRIPT\_LINT\-MEDIUM\] \_\_init\_\_\.py has no function definitions \(flat script\) in /workspace/skills/skill\-creator/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] \_\_init\_\_\.py missing shebang line in /workspace/skills/skill\-creator/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] \_\_init\_\_\.py may lack input validation in /workspace/skills/skill\-creator/scripts/\_\_init\_\_\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] aggregate\_benchmark\.py contains magic numbers in /workspace/skills/skill\-creator/scripts/aggregate\_benchmark\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] generate\_report\.py contains magic numbers in /workspace/skills/skill\-creator/scripts/generate\_report\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] improve\_description\.py contains magic numbers in /workspace/skills/skill\-creator/scripts/improve\_description\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] quick\_validate\.py contains magic numbers in /workspace/skills/skill\-creator/scripts/quick\_validate\.py

**Warning:** \[SCRIPT\_LINT\-MEDIUM\] run\_eval\.py has deeply nested code \(depth 9, max 6\) in /workspace/skills/skill\-creator/scripts/run\_eval\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] run\_eval\.py contains magic numbers in /workspace/skills/skill\-creator/scripts/run\_eval\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] run\_loop\.py contains magic numbers in /workspace/skills/skill\-creator/scripts/run\_loop\.py

**Warning:** \[SCRIPT\_LINT\-LOW\] utils\.py missing shebang line in /workspace/skills/skill\-creator/scripts/utils\.py

## skills/slack\-gif\-creator

[Skill details](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html#skill-017) · [Native HTML](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-017/skillevaluator-tier1.html) · [JSON](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/skill-017/skillevaluator-tier1.json)

### Recorded quality dimensions

| Dimension | Score / 100 | Weight | Issues |
| --- | --- | --- | --- |
| correctness | 85 | 0\.35 | 3 |
| discoverability | 90 | 0\.25 | 2 |
| reliability | 85 | 0\.25 | 3 |
| efficiency | 100 | 0\.15 | 0 |

### Validator outcomes

| Validator | Outcome | Checks recorded | Errors | Warnings |
| --- | --- | --- | --- | --- |
| Schema &amp; Repository Governance | FAIL | 7 | 1 | 6 |
| Semantic Version Validation | NOT APPLICABLE | 1 | 0 | 0 |
| Security Scan | INCOMPLETE | 0 | 1 | 6 |
| PII Scan | PASS | 2 | 0 | 0 |
| License Compliance | PASS | 1 | 0 | 0 |
| Code Risk Analysis | PASS | 2 | 0 | 0 |
| Secrets Detection | PASS | 1 | 0 | 0 |
| Code Integrity &amp; Hygiene | PASS | 5 | 0 | 1 |
| Dependency Vulnerability Audit | INCOMPLETE | 0 | 0 | 4 |
| Unicode Smuggling Detection | PASS | 1 | 0 | 0 |
| QUALITY | PASS | 1 | 0 | 8 |
| SCRIPT\_LINT | NOT APPLICABLE | 1 | 0 | 0 |

### Schema &amp; Repository Governance — evidence

**Evidence: manifest\_exists:** Found skill manifest: SKILL\.md

**Evidence metadata:** \{"file\_path": "/workspace/skills/slack\-gif\-creator/SKILL\.md"\}

**Evidence: frontmatter\_valid:** Valid frontmatter for skill 'slack\-gif\-creator'

**Evidence metadata:** \{"description\_length": 227\}

**Evidence: folder\_hierarchy:** Valid general skill structure: skills/slack\-gif\-creator/

**Evidence: naming\_convention:** Folder name 'slack\-gif\-creator' follows kebab\-case convention

**Evidence metadata:** \{"name\_length": 17\}

**Evidence: line\_count:** SKILL\.md within line limit \(254/500\)

**Evidence metadata:** \{"limit": 500, "line\_count": 254\}

**Evidence: body\_heading:** Body contains a top\-level heading

**Evidence: name\_consistency:** Directory name matches frontmatter: 'slack\-gif\-creator'

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Instructions'

**File:** /workspace/skills/slack\-gif\-creator/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Instructions' or '\#\# Usage' section\. Per agentskills\.io the body format is unrestricted, so this is a convention nudge — it also gives the quality scorer a stable anchor for instruction\-quality heuristics\.

**Finding metadata:** \{"missing\_section": "\#\# Instructions"\}

**Finding: body\_recommended\_section \(medium\):** Missing recommended section: '\#\# Examples'

**File:** /workspace/skills/slack\-gif\-creator/SKILL\.md

**Suggested fix:** Consider adding a '\#\# Examples' section\. If examples are already inline under instructions, this can be skipped\.

**Finding metadata:** \{"missing\_section": "\#\# Examples"\}

**Finding: unexpected\_file \(low\):** Unexpected 'requirements\.txt' in skill root

**File:** /workspace/skills/slack\-gif\-creator/requirements\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'core' in skill root

**File:** /workspace/skills/slack\-gif\-creator/core

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: unexpected\_file \(low\):** Unexpected 'LICENSE\.txt' in skill root

**File:** /workspace/skills/slack\-gif\-creator/LICENSE\.txt

**Suggested fix:** Consider moving to one of: agents/, assets/, config/, evals/, references/, scripts/, tests/, tools/\. To allow additional directories, set $SKILLEVALUATOR\_SCHEMA\_ALLOWED\_DIRS\.

**Finding: author\_missing \(high\):** Author not specified in metadata

**File:** /workspace/skills/slack\-gif\-creator/SKILL\.md

**Suggested fix:** Add 'metadata\.author' field with format 'Name &lt;email@​example\.com&gt;'

**Finding metadata:** \{"profile": "external"\}

**Error:** \[SCHEMA\-HIGH\] Author not specified in metadata in /workspace/skills/slack\-gif\-creator/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Instructions' in /workspace/skills/slack\-gif\-creator/SKILL\.md

**Warning:** \[SCHEMA\-MEDIUM\] Missing recommended section: '\#\# Examples' in /workspace/skills/slack\-gif\-creator/SKILL\.md

**Warning:** \[SCHEMA\-LOW\] Unexpected 'requirements\.txt' in skill root in /workspace/skills/slack\-gif\-creator/requirements\.txt

**Warning:** \[SCHEMA\-LOW\] Unexpected 'core' in skill root in /workspace/skills/slack\-gif\-creator/core

**Warning:** \[SCHEMA\-LOW\] Unexpected 'LICENSE\.txt' in skill root in /workspace/skills/slack\-gif\-creator/LICENSE\.txt

**Warning:** Workflow scope: llm skipped\. LLM checks disabled by \-\-no\-llm\.

**Scanner message:** \[OK\] manifest\_exists: Found skill manifest: SKILL\.md

**Scanner message:** \[OK\] frontmatter\_valid: Valid frontmatter for skill 'slack\-gif\-creator'

**Scanner message:** \[OK\] folder\_hierarchy: Valid general skill structure: skills/slack\-gif\-creator/

**Scanner message:** \[OK\] naming\_convention: Folder name 'slack\-gif\-creator' follows kebab\-case convention

**Scanner message:** \[OK\] line\_count: SKILL\.md within line limit \(254/500\)

**Scanner message:** \[OK\] body\_heading: Body contains a top\-level heading

**Scanner message:** \[OK\] name\_consistency: Directory name matches frontmatter: 'slack\-gif\-creator'

### Semantic Version Validation — evidence

**Evidence: version\_optional:** No semantic version label present; resource will use commit\-hash history

**Evidence metadata:** \{"previous\_version": null\}

**Scanner message:** \[OK\] version\_optional: No semantic version label present; resource will use commit\-hash history

### Security Scan — evidence

**Finding: Unpinned Dependencies \(SC1\) \(low\):** Supply Chain: pillow&gt;=10\.0\.0

**File:** requirements\.txt

**Line:** 1

**Source line:** pillow&gt;=10\.0\.0 imageio&gt;=2\.31\.0 imageio\-ffmpeg&gt;=0\.4\.9 numpy&gt;=1\.24\.0

**Suggested fix:** Dependencies lack version pinning, allowing potential malicious package updates\. Consider pinning versions\. Pin all dependency versions in requirements\.txt or pyproject\.toml\. Use exact versions \(==\) or compatible ranges\. Run pip\-audit regularly\.

**Finding metadata:** \{"skillspector\_confidence": 0\.5\}

**Finding: Unverifiable Dependency: pillow has 16 known advisory\(ies\) \(CVE\-2026\-112390 \(Pillow: Infinite loop in MIC n\_frames when the embedded TIFF\); CVE\-2026\-96638 \(Pillow: BMP RLE decoder memory\-amplification DoS via unbounded delta escape / ab\); CVE\-2026\-112391 \(Pillow: PdfParser can recurse without limit in get\_value\(\) and linearize\_page\_tr\) \+13 more\), but the manifest does not pin a version, so it is unknown whether the installed release is affected \(SC4\) \(low\):** Supply Chain: pillow

**File:** requirements\.txt

**Line:** 1

**Suggested fix:** Dependency has known vulnerabilities \(CVEs\)\. Using packages with unpatched security flaws exposes the environment to known exploits\. Update the dependency to a patched version that addresses the known CVE\. Check OSV \(osv\.dev\) or NVD for details on the vulnerability\.

**Finding metadata:** \{"skillspector\_confidence": 0\.4\}

**Finding: Unpinned Dependencies \(SC1\) \(low\):** Supply Chain: imageio&gt;=2\.31\.0

**File:** requirements\.txt

**Line:** 2

**Truncated for CI display limits. Full evidence remains in the HTML report and raw JSON/log artifacts.**

[Open full report](https://chrisknvidia.github.io/skillevaluator-cli-playground/runs/41559367506/1/index.html) · [Workflow run and logs](https://github.com/chrisknvidia/skillevaluator-cli-playground/actions/runs/41559367506)
