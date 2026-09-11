# App-Building Questions for Agents

A 10-question discovery questionnaire for scoping a new application project.

## What this repo is

This repo's primary artifact is the questionnaire: [`docs/QUESTIONNAIRE.md`](docs/QUESTIONNAIRE.md). It is a lightweight requirements-discovery framework — answer the ten questions to align stakeholders and guide early technical decisions (platform, language, must-have MVP features, integrations, data, security, UX tone, scale, and budget/timeline). The legacy root-level copy [`10 Questions to help you build an app.md`](./10%20Questions%20to%20help%20you%20build%20an%20app.md) is kept for backward-compatible inbound links only.

## Contents

1. [Q1. What problem does your application solve, and who feels that pain the most?](docs/QUESTIONNAIRE.md#q1-what-problem-does-your-application-solve-and-who-feels-that-pain-the-most)
2. [Q2. On which devices and platforms should the first version run?](docs/QUESTIONNAIRE.md#q2-on-which-devices-and-platforms-should-the-first-version-run)
3. [Q3. Which scripting/programming language(s) do you prefer, and why?](docs/QUESTIONNAIRE.md#q3-which-scriptingprogramming-languages-do-you-prefer-and-why)
4. [Q4. List the must-have features for the MVP (Minimum Viable Product)?](docs/QUESTIONNAIRE.md#q4-list-the-must-have-features-for-the-mvp-minimum-viable-product)
5. [Q5. Which third-party services or APIs should we integrate with (if any)?](docs/QUESTIONNAIRE.md#q5-which-third-party-services-or-apis-should-we-integrate-with-if-any)
6. [Q6. How should data be stored and synced?](docs/QUESTIONNAIRE.md#q6-how-should-data-be-stored-and-synced)
7. [Q7. What level of security, privacy, or compliance is required?](docs/QUESTIONNAIRE.md#q7-what-level-of-security-privacy-or-compliance-is-required)
8. [Q8. How should the user interface feel (style, tone, accessibility)?](docs/QUESTIONNAIRE.md#q8-how-should-the-user-interface-feel-style-tone-accessibility)
9. [Q9. What are your performance or scalability expectations for the first year?](docs/QUESTIONNAIRE.md#q9-what-are-your-performance-or-scalability-expectations-for-the-first-year)
10. [Q10. Budget, timeline, and post-launch maintenance — what's realistic?](docs/QUESTIONNAIRE.md#q10-budget-timeline-and-post-launch-maintenance-whats-realistic)

## How to use it

1. Open the questionnaire file.
2. For each question, pick the example answer closest to your situation — or write your own.
3. Drop your answers into a shared doc, then derive functional + non-functional requirements.
4. Use the "Deliverables Checklist" at the bottom of the questionnaire as a starting point for downstream artifacts (architecture diagram, roadmap, budget breakdown, testing strategy, deployment plan).

## Repo contents

| Path | What it is |
|------|------------|
| `10 Questions to help you build an app.md` | Legacy root-level questionnaire (kept for backward-compatible inbound links; canonical content now lives at `docs/QUESTIONNAIRE.md`). |
| `CONTRIBUTING.md` | How to add, edit, or refine a question; style guide and contribution workflow. |
| `LICENSE` | MIT licence, © 2026 TeacherEvan. |
| `README.md` | This file — entry point: title, contents, links, how to use. |
| `.snapshots/` | Third-party configuration and docs for the **Snapshots-for-AI** VSCode/Cursor extension by [GBTI Network](https://gbti.network). It is auto-managed by the extension; this repo does not own or maintain it. |
| `docs/QUESTIONNAIRE.md` | Canonical 10-question discovery framework. |
| `docs/INDEX.md` | Documentation index: every markdown file in this repo, with a one-line summary. |
| `docs/.scratch-audit/` | Internal V2 governance run artifacts (gitignored, ephemeral). |

## Contributing

This is a content template — there is no application code to run or test. If you want to propose changes to the questionnaire:

1. Open the questionnaire file and make your edits.
2. Open a PR with a clear rationale (e.g., "add a question about accessibility defaults", "rework Q4 MVP examples").
3. Keep the heading hierarchy and example-answer format intact so the file remains easy to copy-paste into a fresh doc.

## Why "for Agents" in the repo name?

The questionnaire is intended to be usable by both humans and AI coding assistants — the questions are framed at a level of abstraction that works as a prompt seed for downstream agentic workflows (scoping an MVP, picking a stack, drafting a roadmap). The name reflects that scope; the artifact itself is human-first.

## License

This repo is licensed under the [MIT licence](LICENSE) (c) 2026 TeacherEvan. See `LICENSE` for the full text.
