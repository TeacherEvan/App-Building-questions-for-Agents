# App-Building Questions for Agents

A 10-question discovery questionnaire for scoping a new application project.

## What this repo is

This repo hosts a single markdown file: [`10 Questions to help you build an app.md`](./10%20Questions%20to%20help%20you%20build%20an%20app.md). It is a lightweight requirements-discovery framework — answer the ten questions to align stakeholders and guide early technical decisions (platform, language, must-have MVP features, integrations, data, security, UX tone, scale, and budget/timeline).

## How to use it

1. Open the questionnaire file.
2. For each question, pick the example answer closest to your situation — or write your own.
3. Drop your answers into a shared doc, then derive functional + non-functional requirements.
4. Use the "Deliverables Checklist" at the bottom of the questionnaire as a starting point for downstream artifacts (architecture diagram, roadmap, budget breakdown, testing strategy, deployment plan).

## Repo contents

| Path | What it is |
|------|------------|
| `10 Questions to help you build an app.md` | The questionnaire (the actual artifact). |
| `.snapshots/` | Third-party configuration and docs for the **Snapshots-for-AI** VSCode/Cursor extension by [GBTI Network](https://gbti.network). It is auto-managed by the extension; this repo does not own or maintain it. |
| `LICENSE` | Not present — author license intent is unspecified. Treat content as all-rights-reserved unless the author clarifies otherwise. |
| `docs/.scratch-audit/` | Internal V2 governance run artifacts (gitignored, ephemeral). |

## Contributing

This is a content template — there is no application code to run or test. If you want to propose changes to the questionnaire:

1. Open the questionnaire file and make your edits.
2. Open a PR with a clear rationale (e.g., "add a question about accessibility defaults", "rework Q4 MVP examples").
3. Keep the heading hierarchy and example-answer format intact so the file remains easy to copy-paste into a fresh doc.

## Why "for Agents" in the repo name?

The questionnaire is intended to be usable by both humans and AI coding assistants — the questions are framed at a level of abstraction that works as a prompt seed for downstream agentic workflows (scoping an MVP, picking a stack, drafting a roadmap). The name reflects that scope; the artifact itself is human-first.

## License

No `LICENSE` file is present. Unless the author adds one, reuse is at your own risk — please ask before redistributing.
