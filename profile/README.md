# Aelira AI

**Accessibility remediation for course content. It returns fixed files, not a list of problems.**

Aelira helps universities and colleges meet WCAG 2.1 AA, including the US DOJ ADA Title II deadlines (26 April 2027 for large public entities, 26 April 2028 for smaller ones). Most tools tell you a PDF has no tags; Aelira gives you back a remediated file, with a report of what changed and why.

## Projects

### [aelira-core](https://github.com/Aelira-AI/aelira-core)
The engine and dashboard — FastAPI backend, React dashboard, and the command-line tool, all in one repo with one CI run. Scans and remediates PDFs, Word, PowerPoint, Excel, LaTeX, web pages, images, and video. Reads course content directly from Canvas, Blackboard, Moodle, and Brightspace over LTI 1.3, plus Google Drive and Microsoft 365. **AGPL-3.0** (CLI under `cli/` is MIT).

## What makes Aelira different

- **Severity is computed, not generated.** A plain function of the rule that fired — the same file produces the same result on every scan. There's a test that fails if it ever doesn't.
- **Remediation over reporting.** You get fixed files and written-back LMS content, review-gated with an audit log and rollback.
- **Bring your own model.** Gemini, OpenAI, Anthropic, xAI, any OpenAI-compatible endpoint — or fully local via Ollama, where documents never leave your servers.
- **Genuinely self-hostable.** One `docker compose` command to try it; the open core is the full engine, not a demo.

## Get involved

Contributions welcome — start with the [contributing guide](https://github.com/Aelira-AI/aelira-core/blob/main/CONTRIBUTING.md) and the [developer onboarding](https://github.com/Aelira-AI/aelira-core/blob/main/docs/development/onboarding.md).

- [Report a bug](https://github.com/Aelira-AI/aelira-core/issues/new?template=bug_report.md)
- [Request a feature](https://github.com/Aelira-AI/aelira-core/issues/new?template=feature_request.md)
- [Security policy](https://github.com/Aelira-AI/aelira-core/blob/main/SECURITY.md)

## Links

- [aelira.ai](https://aelira.ai) — the hosted service
- [Self-hosting guide](https://github.com/Aelira-AI/aelira-core/blob/main/docs/deployment/self-hosting.md)
