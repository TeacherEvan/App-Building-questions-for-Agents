# Application Discovery Questionnaire — App Building Questions for Agents

A focused 10-question framework for aligning stakeholders before any software project
kicks off. Use it to derive requirements, scope, and architecture decisions from a
shared conversation.

## What this repo is

- **A questionnaire.** Ten questions every project should answer before writing code.
- **A `.snapshots/` integration.** Bundled configuration for the Snapshots-for-AI tool,
  which lets you ship project context to an AI assistant in a single prompt.

## Contents

The full questionnaire lives at [`docs/QUESTIONNAIRE.md`](docs/QUESTIONNAIRE.md).
For convenience, an index of every doc is in [`docs/INDEX.md`](docs/INDEX.md).

Quick links:

| # | Question | Why we ask |
|---|----------|------------|
| Q1 | [What problem does your application solve, and who feels that pain the most?](docs/QUESTIONNAIRE.md#q1-what-problem-does-your-application-solve-and-who-feels-that-pain-the-most) | Defines the core value proposition and primary users. |
| Q2 | [On which devices and platforms should the first version run?](docs/QUESTIONNAIRE.md#q2-on-which-devices-and-platforms-should-the-first-version-run) | Narrows the tech stack and design constraints. |
| Q3 | [Which scripting/programming language(s) do you prefer, and why?](docs/QUESTIONNAIRE.md#q3-which-scriptingprogramming-languages-do-you-prefer-and-why) | Aligns with existing team skill, hosting options, and library ecosystems. |
| Q4 | [List the must-have features for the MVP (Minimum Viable Product).](docs/QUESTIONNAIRE.md#q4-list-the-must-have-features-for-the-mvp-minimum-viable-product) | Prevents scope creep; anchors the first release. |
| Q5 | [Which third-party services or APIs should we integrate with (if any)?](docs/QUESTIONNAIRE.md#q5-which-third-party-services-or-apis-should-we-integrate-with-if-any) | Determines licensing cost, data flow, and potential vendor lock-in. |
| Q6 | [How should data be stored and synced?](docs/QUESTIONNAIRE.md#q6-how-should-data-be-stored-and-synced) | Guides database choice, offline strategy, and security controls. |
| Q7 | [What level of security, privacy, or compliance is required?](docs/QUESTIONNAIRE.md#q7-what-level-of-security-privacy-or-compliance-is-required) | Impacts architecture, hosting region, and audit features. |
| Q8 | [How should the user interface feel (style, tone, accessibility)?](docs/QUESTIONNAIRE.md#q8-how-should-the-user-interface-feel-style-tone-accessibility) | Sets design language and accessibility targets. |
| Q9 | [What are your performance or scalability expectations for the first year?](docs/QUESTIONNAIRE.md#q9-what-are-your-performance-or-scalability-expectations-for-the-first-year) | Determines hosting tier, caching, and cost planning. |
| Q10 | [Budget, timeline, and post-launch maintenance — what's realistic?](docs/QUESTIONNAIRE.md#q10-budget-timeline-and-post-launch-maintenance-whats-realistic) | Aligns scope with resources and clarifies ongoing responsibilities. |

## How to use

1. Open [`docs/QUESTIONNAIRE.md`](docs/QUESTIONNAIRE.md) and answer each question in order.
2. Use the example answers as scaffolding — adapt them to your context, don't copy them verbatim.
3. After completing, distill the answers into:
   - a requirements document (functional + non-functional),
   - an architecture diagram,
   - a phased roadmap,
   - a budget breakdown,
   - a maintenance plan post-launch.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) if you want to add, edit, or refine a question.

## Snapshots integration

The `.snapshots/` directory bundles configuration for [Snapshots-for-AI](.snapshots/readme.md),
a tool that packages your project context for an AI assistant. See `.snapshots/readme.md`
for setup, `.snapshots/config.json` for the current configuration, and
`.snapshots/sponsors.md` for third-party tool sponsorships.

## Licence

[MIT](LICENSE)

## Question Reference

For searchability and direct deep-linking from external tools, every question has
its own section here.

## Q1

See [`docs/QUESTIONNAIRE.md#q1-what-problem-does-your-application-solve-and-who-feels-that-pain-the-most`](docs/QUESTIONNAIRE.md#q1-what-problem-does-your-application-solve-and-who-feels-that-pain-the-most).

## Q2

See [`docs/QUESTIONNAIRE.md#q2-on-which-devices-and-platforms-should-the-first-version-run`](docs/QUESTIONNAIRE.md#q2-on-which-devices-and-platforms-should-the-first-version-run).

## Q3

See [`docs/QUESTIONNAIRE.md#q3-which-scriptingprogramming-languages-do-you-prefer-and-why`](docs/QUESTIONNAIRE.md#q3-which-scriptingprogramming-languages-do-you-prefer-and-why).

## Q4

See [`docs/QUESTIONNAIRE.md#q4-list-the-must-have-features-for-the-mvp-minimum-viable-product`](docs/QUESTIONNAIRE.md#q4-list-the-must-have-features-for-the-mvp-minimum-viable-product).

## Q5

See [`docs/QUESTIONNAIRE.md#q5-which-third-party-services-or-apis-should-we-integrate-with-if-any`](docs/QUESTIONNAIRE.md#q5-which-third-party-services-or-apis-should-we-integrate-with-if-any).

## Q6

See [`docs/QUESTIONNAIRE.md#q6-how-should-data-be-stored-and-synced`](docs/QUESTIONNAIRE.md#q6-how-should-data-be-stored-and-synced).

## Q7

See [`docs/QUESTIONNAIRE.md#q7-what-level-of-security-privacy-or-compliance-is-required`](docs/QUESTIONNAIRE.md#q7-what-level-of-security-privacy-or-compliance-is-required).

## Q8

See [`docs/QUESTIONNAIRE.md#q8-how-should-the-user-interface-feel-style-tone-accessibility`](docs/QUESTIONNAIRE.md#q8-how-should-the-user-interface-feel-style-tone-accessibility).

## Q9

See [`docs/QUESTIONNAIRE.md#q9-what-are-your-performance-or-scalability-expectations-for-the-first-year`](docs/QUESTIONNAIRE.md#q9-what-are-your-performance-or-scalability-expectations-for-the-first-year).

## Q10

See [`docs/QUESTIONNAIRE.md#q10-budget-timeline-and-post-launch-maintenance-whats-realistic`](docs/QUESTIONNAIRE.md#q10-budget-timeline-and-post-launch-maintenance-whats-realistic).
