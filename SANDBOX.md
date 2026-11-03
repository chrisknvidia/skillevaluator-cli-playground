# SkillEvaluator onboarding playground

This personal sandbox lets you try a local interactive wizard for automatic skill checks, hosted HTML reports, and updated PR comments.

Start the local **START.command** launcher supplied with the sandbox. Choose **sandbox-skills** for the first run: it contains two small text-only demonstration skills. The wizard configures GitHub and opens a setup PR. Review and merge that PR, then open a new PR changing a selected skill. The check, report and comment follow automatically.

The sample skills are copied from NVIDIA/SkillEvaluator's public `ci/smoke_image.py` fixtures (CI release source `e4cda13a85f34fa7a112b3529feaf24cfe587caf`). Their manifests declare MIT licensing. Existing upstream files and workflows remain available.

The scanner image is the official static CI release. The publisher is an immutable review candidate from NVIDIA/SkillEvaluator#326; the local wizard is experimental and is not part of the installed Python package. No model key or personal token needs to be pasted into the wizard. It reuses the existing GitHub CLI login. Reports on this public sandbox's Pages site are public.
