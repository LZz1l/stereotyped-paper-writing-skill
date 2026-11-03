# Stereotyped Paper Writing Skill

An English academic-writing skill for Codex. It turns a research paper into a connected argument: problem → gap → method → evidence → meaning.

The name refers to a reusable section structure. The scientific claims, results, and decisions still come from the research and its authors.

## What it does

- A four-sentence abstract: field, scientific problem, method with quantitative evidence, and value.
- A four-paragraph funnel introduction: context, prior work, gap, and approach with contributions.
- Overview-first methods: a framework figure, module explanations, motivated equations, and precise novelty.
- Contribution-focused experiments: comparison tables with venues and metric directions, a separate ablation subsection, and readable visuals using light colors.
- An optional discussion and a concise conclusion without repeating content already discussed.
- Confident, contribution-first English without repetitive defensive or procedural prose.

The user owns consequential choices, including what to omit or decline. The skill asks focused questions, waits for decisions that affect the work, and continues independent authorized tasks. It does not invent evidence or treat writing permission as permission to run experiments or publish a paper.

## Install

Clone this repository into a skill folder. The destination must not already exist:

```sh
git clone https://github.com/LZz1l/stereotyped-paper-writing-skill.git \
  ~/.agents/skills/stereotyped-paper-writing-skill
```

The current [official Codex skills documentation](https://learn.chatgpt.com/docs/build-skills) lists `~/.agents/skills` for user skills. If your existing Codex installation discovers user skills in `~/.codex/skills`, use that directory instead. Install one copy in the location your host discovers. The installed folder must contain `SKILL.md` directly. If the skill does not appear after installation, restart Codex.

## Use

Invoke the skill explicitly in a Codex chat:

```text
Use $stereotyped-paper-writing-skill to revise my abstract and introduction.
Preserve my scientific claims. Ask me before changing the contribution
positioning, excluding substantive content, or adding experiments.
```

Or ask for a complete manuscript task:

```text
Use $stereotyped-paper-writing-skill to help write my English paper.
Read the supplied draft, results, and references first. Ask me about the
important missing facts and choices, then complete the agreed sections.
```

Provide the draft or research materials, available evidence, target venue if known, and editing scope. Missing facts lead to questions, not invented results. Ordinary automatic skill selection remains enabled by default; explicit invocation makes the choice clear.

## Files

- [`SKILL.md`](SKILL.md): the complete writing and decision workflow.
- [`agents/openai.yaml`](agents/openai.yaml): Codex display metadata and example invocation.
- [`LICENSE`](LICENSE): MIT license.

No external tools, paid APIs, scripts, or additional skills are required by this skill. Tools for literature lookup, figure production, or manuscript rendering depend on the task and the host environment.

## License

MIT. See [LICENSE](LICENSE).
