# Contributing

Thanks for considering a contribution to the Application Discovery Questionnaire.

The questionnaire is intentionally short (10 questions). Adding or refining a question
has wide downstream impact — please read this guide first.

## How to add a question

1. **Open an issue** describing the gap. A new question should cover a decision the
   current ten miss; if a current question can be reworded to absorb the gap, prefer
   that and skip step 2.
2. **Edit `docs/QUESTIONNAIRE.md`** (canonical). Keep the new question aligned with
   the format of the existing ten — a `### Q<N>. <Title Case Question>?` heading,
   a `**Why we ask:** ...` rationale, and 2–3 example answers.
3. **Update `README.md`** so the contents table includes the new question with its
   anchor link, then update `docs/INDEX.md` if any new supporting doc was added.
4. **Mirror the change in the legacy file** `10 Questions to help you build an app.md`
   so inbound links still resolve to the same content.
5. **Open a pull request** with a one-paragraph rationale and a checklist confirming
   `docs/QUESTIONNAIRE.md`, `README.md`, and the legacy file are all updated.

## How to refine an existing question

1. **Edit `docs/QUESTIONNAIRE.md`** (canonical).
2. **Mirror the change in the legacy file** `10 Questions to help you build an app.md`.
3. **Open a pull request** explaining the rationale and any backward-compatibility notes.

## Style

- Headings: `### Q<N>. <Title Case Question>?`
- Question text must end with a question mark.
- One `**Why we ask:**` line directly under the heading.
- 2–3 example answers, in plain prose, prefixed with `- "..."` (or `- **Label** – "..."`).
- One blank line between questions; no trailing whitespace.

## Licence

By contributing, you agree your contributions are licensed under the MIT licence
(see [`LICENSE`](LICENSE)).
