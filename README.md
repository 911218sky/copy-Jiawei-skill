# Copy Jiawei Skill

A portable Markdown skill for **Jiawei-style first-principles seminar questioning** — single-thread depth, teach-then-verify, guess-before-lookup, table-aware live Q, and constructive closure.

**Version:** 1.1.0

## What it does

- Clarifies **output target** (L0) when architecture slides hide what is predicted.
- Traces **why** a method or assumption was chosen, not only **how** it works.
- Tests whether core premises match the **actual operating regime** (L2).
- Checks whether inputs match **expert practice** (L3) and who counts as **ground truth** (L4).
- Runs **constraint archaeology** and **present-vs-past delta** when "it was fine back then" (L5a/L5b).
- When live with slides: **anchors doubt to tables** (H12), reads **pre-add vs post-add** rows (H10), and checks the **community benchmark bar** (H11).
- Uses a **non-linear trigger graph** — layer order follows answer quality, not a fixed checklist.
- Applies **twelve** named heuristics (H1–H12) reactively, including teach-then-verify and good-start closure.
- Enforces **decision-relevance** and **stop rules** so live Q&A opens one thread, not an interrogation.
- Closes with **exactly one offline homework** and affirms progress.

This skill is **thinking protocol only**. It does not search literature, cite papers, or embed domain-specific seminar examples.

## Modes

`standard` is the default single-thread workflow. Use `deep` when the thread needs the fuller arc — including H2, H5, temporal L5a/L5b, H7, and **L0 / H10–H12 only when** architecture, ablation, split, or slides triggers fire. Use `debrief` for post-seminar write-ups. Use `prep` to generate live lines before a talk. All modes use **one mentor voice** — layers and heuristics are internal moves, not separate roles.

Example request:

> Use `deep` mode like Jiawei: pick one thread on this seminar report, run the trigger graph, and give me 2 live questions plus one homework.

## Trigger-graph design (v1.1.0)

Version 1.1.0 packages Jiawei's mentoring logic as:

- **Phase map**: Gate & packet → optional L0 → origin & premise → branch & compare (incl. H10–H12 when triggered) → ownership & temporal (L5 only on temporal excuse) → closure.
- **Twelve heuristics**: H1–H12 as distinct cognitive jobs (not tone variants); invoke reactively, never as a shopping list.
- **Context tuning**: Adjust depth by talk type (first report, methods, legacy design, paper selection, ablation, live slides).
- **Mentor norms**: Single-thread, decision-relevance gate, tables-over-narrative, guess-before-lookup, no live literature cosplay.

See [`reference.md`](reference.md) for the trigger graph, question bank, reactive playbook, and quality rubric.

## Installation

Copy the skill directory into any Agent or assistant environment that supports Markdown-based skills. The runtime only needs to read `SKILL.md`; no package manager or platform integration is required.

Example layout:

```text
skills/
└── copy-Jiawei-skill/
    ├── SKILL.md
    ├── README.md
    ├── reference.md
    ├── CHANGELOG.md
    └── LICENSE
```

After installation, ask the assistant to question a seminar report, prepare live Q&A, or debrief using Jiawei's logic.

## Scope

General-purpose seminar questioning skill. Not tied to a research field, project, or specific past talk. When the domain is unknown, use generic question stems from `reference.md`; do not invent domain filler.

## License

GNU Affero General Public License v3.0 or later. See [`LICENSE`](LICENSE).
