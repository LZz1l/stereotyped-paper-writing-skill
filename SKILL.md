---
name: stereotyped-paper-writing-skill
description: Draft, revise, and review English research papers using a four-part abstract, four-paragraph funnel introduction, overview-first methods, and contribution-focused experiments. Use for structured academic manuscript writing and editing while keeping consequential choices with the user.
---

# Stereotyped Paper Writing

Write English research papers around one continuous argument: scientific problem → gap → method → evidence → meaning. Use the section structures below as the default writing framework. Let the user's current instructions, confirmed decisions, and actual venue requirements determine any adaptations. This skill provides a rhetorical structure, not canned claims or permission to conduct research.

## Keep decisions with the user

Ask more when the answer changes the paper; do not ask merely to fill a quota.

- Read the supplied manuscript, research materials, and existing decisions before asking. Establish the requested deliverable, sections, contribution, evidence available, target venue if known, and editing boundaries.
- When direction or an important choice is unresolved, offer a recommendation with a short reason and meaningful alternatives. Ask 2–4 focused questions per round when that many matter; accept free-form answers. Do not repeat questions already answered.
- The user decides the central claim, contribution positioning, assumptions, scope, inclusion or exclusion of substantive content, research direction, and whether to add or run experiments. This includes **decisions about what not to do**: do not silently drop a requested section, reject a method, remove evidence, abandon an experiment, or narrow the assignment.
- If material seems unrelated, weak, redundant in a consequential way, or inconsistent with the main argument, explain its role and propose a concrete treatment. Ask before making a substantive omission or reframing the claim. Routine wording edits and deduplication already authorized by the user can proceed.
- Wait for an answer before doing work that depends on a consequential choice. Silence is not consent. Continue independent, authorized work and identify the precise dependency.
- Once choices are confirmed, complete the authorized work and its checks continuously. Do not turn routine execution into repeated requests to continue. Do not substitute an outline or partial draft for a requested complete manuscript.
- Writing authorization alone does not authorize new experiments, source-code changes, publication, or external messages. Propose additional work and let the user decide.

Communicate questions and progress in the user's preferred language; write manuscript prose in English unless the user requests otherwise. For a narrow edit, preserve the existing argument and unrelated text. Ask only for facts needed by that edit; missing paper-wide context must not block wording that is fully supported by the supplied material.

## Establish the argument before drafting

From the available material, identify the scientific question, the specific gap, the mechanism that addresses it, the evidence supporting each contribution, and the resulting scientific or practical value. A short private outline is sufficient; avoid imposing a new process on a small edit.

If one of these is unknown, ask about the missing fact rather than inventing a connection. Distinguish an expression problem from missing implementation or missing evidence. A polished sentence cannot resolve the latter two.

Use only supplied or verified results and sources. Never invent numerical gains, datasets, baselines, significance, citations, venues, publication years, proofs, or novelty claims. Do not turn expected outcomes into measured results. In a working draft, use clearly marked placeholders only when the user wants a scaffold; never present them as publication-ready text. Do not infer that a contribution is unprecedented because a search found no match.

## Abstract: four sentences forming a closed loop

1. **Field and background.** Name the research field and the relevant setting directly. Give only the background needed to understand the problem.
2. **Scientific problem.** State the concrete unresolved problem in that field. Make clear what current approaches cannot adequately explain or accomplish, using accurate, supported language.
3. **Method and quantitative answer.** State the proposed method and its key mechanism, then report representative simulation or experimental results with real quantitative metrics. Include the comparison or conditions needed to interpret the numbers. Explain how the result answers the problem in sentence 2.
4. **Value.** Explain the scientific significance or practical application enabled by that answer. End with what the work contributes.

Default to four sentences, with sentence 3 connecting method and evidence. If a word limit, complex result, or theory-only paper calls for a different form, propose a specific adaptation and ask before changing this structure. When results are missing, request them and continue other supported sections; do not manufacture a quantitative abstract. Offer a result-free method or proposal abstract as an optional adaptation if useful, and wait for the user's choice; do not label it an experimentally validated final abstract.

## Introduction: a four-paragraph funnel

1. **Broad context → specific setting → value.** Narrow from the broader research context to the concrete setting and explain why solving the problem matters. Establish the reader's motivation without a long generic opening.
2. **Relevant prior work.** Organize the most relevant research by approach or capability. Explain what it established and how that progress leads to the present problem; avoid an unrelated citation list.
3. **Gap, challenges, and necessity.** Identify the precise remaining gap and the scientific or technical challenges behind it. Show why existing results leave this problem unresolved and why this paper is needed. Represent earlier work fairly.
4. **Approach and contributions.** Explain how the method addresses that gap and state the core contributions. Connect each contribution to a problem and a supported result rather than listing implementation tasks.

Keep four paragraphs by default. If a venue requires a separate contribution list, attach it to the fourth paragraph without creating a second storyline. Ask before adopting a materially different introduction structure.

## Methods: the whole algorithm before its details

### Start with an overview and a main figure

Explain the complete algorithm before local derivations. State how many modules it has, what each module does, and the ordered steps from input to output. Explain their dependencies and how the combined process solves the research problem.

Provide a main **Framework** or **Overview** figure showing inputs, outputs, module roles, directional flow, and all core innovations in their actual locations. The figure should make the method understandable before the reader studies the equations. Use consistent module names in the figure, prose, and subsections. If the mechanism is unclear, ask before drawing it. When figure production is outside the authorized deliverable, supply a concrete figure specification and explain the remaining production step; do not claim an image exists.

### Expand by module

For each module, explain in a connected sequence:

- What problem it solves.
- What its inputs represent.
- How it processes them, including the relevant computation.
- What it outputs and which next step consumes that output.
- Why this design is appropriate for the stated problem.

Introduce concepts before using them to carry an argument. Keep implementation detail proportional to its role in understanding or reproducing the method.

### Give every equation a purpose

Before an equation, explain the need or question that motivates it. After it, define every newly introduced symbol, including dimensions, domains, indices, and assumptions where needed. Explain what the equation accomplishes and how its result is used next. Do not insert unexplained formulas or repeat definitions of symbols already established clearly.

### Locate the novelty

At the relevant design choice, explain what differs from the closest existing approaches, why that difference addresses the gap, and what would change without it. Distinguish a design rationale from an empirically demonstrated effect. Keep this explanation concise; detailed comparisons and ablations belong in the experiments. If necessity is not established, ask how the user wants to position the design rather than asserting that it is indispensable.

## Experiments: evidence for the central contributions

Organize experiments around questions that test the paper's contributions. For each experiment, connect the research question, comparison or intervention, metric, result, and interpretation. Write the result as an answer to that question, not as a chronological account of runs.

Exclude unrelated or weakly relevant experiments from a proposed experiment plan. For existing or explicitly requested material, explain why it does not support the main argument and obtain the user's decision before omitting it. Do not invent, discard, or conceal results to make the method appear stronger. If an unfavorable result changes a claim, tell the user and ask how to revise the claim or investigate it.

### Comparative evaluation

Most empirical method papers benefit from comparisons. If comparisons have not been addressed, ask whether the user wants comparative experiments, which methods are appropriate, and whether the task is to design them or analyze existing data. Recommend meaningful baselines and fair conditions; do not launch experiments or treat proposed baselines as measured results without authorization. Preserve an already confirmed comparison plan.

Present numerical results in standard, clearly structured tables rather than isolated numbers. For a method-comparison table, use this default column order:

**Method | Venue | Metric A ↑ | Metric B ↓ | …**

- The first column identifies the method. The second gives the verified conference or journal name and publication year, such as `Conference Name 20XX`. Place the supporting citation with the method or venue as the manuscript style requires. Ask for an unknown source; identify a preprint or unpublished method honestly rather than assigning a venue. A clearly labeled working table may use `Source pending`; resolve that cell before presenting the table as final. For the current unpublished method, use an explained dash or `This work`.
- Choose the remaining columns for the actual scientific questions and datasets. Put **↑** or **↓** in each quantitative metric header, or an equally explicit supported equivalent, so readers know whether higher or lower is better. Explain a metric with no simple monotone preference.
- State units, evaluation conditions, and uncertainty where the data support them. Distinguish percentage-point changes from relative percentages. Keep precision consistent and do not manufacture variability or statistical significance.
- Highlight the best and second-best values with distinct pale colors when the venue permits, and explain the convention in the caption. Use additional bold/underline or another clear cue so color is not the only signal. Respect ties, rounding, and uncertainty; do not imply a meaningful winner from unsupported differences.
- Do not mix incompatible evaluation conditions in a ranking. If results come from different sources, make their provenance and comparability clear in concise table notes.

### Separate ablation subsection

Include a distinct ablation subsection for empirical methods with separable design choices. Connect each removal or replacement to a claimed mechanism; report the full method and relevant variants under comparable conditions. State which contribution each comparison supports and what the evidence actually establishes.

When ablation data are missing, ask whether to design the ablations or obtain existing results. Do not silently omit this subsection, invent a completed study, or run it without authorization. If ablation is inapplicable, such as for a purely theoretical contribution, propose a suitable alternative and let the user approve that adaptation.

### Figures and tables

Use a restrained, light palette, clear labels, readable type, balanced spacing, consistent scales, and logical visual grouping. Keep text and axes dark enough to read; avoid heavy fills, decorative clutter, and color-only distinctions. Captions should state the question, comparison, conditions needed for interpretation, and takeaway. Inspect the actual rendered figure or table for clipping, overlap, legibility, and consistency when producing visual artifacts; file generation alone is insufficient.

## Discussion: include when needed

Confirm whether a separate discussion is wanted or required when that decision is unresolved. If included, develop these moves without retelling every result:

1. Reconnect the research question, method, and importance.
2. Interpret the main findings and their implications.
3. Compare the findings with prior research and explain the value of the similarities or differences.
4. Consider plausible alternative explanations and unresolved questions objectively.
5. State substantive limitations once, with their actual effect on interpretation.
6. Suggest future directions that follow from those findings and remaining questions.

Keep this section focused and constructive. Do not add speculative weaknesses, habitual disclaimers, or repeated lists of unfinished work. Explain material boundaries to the user and ask about their placement; do not silently omit facts that determine whether the central conclusion holds.

## Conclusion: judgment and meaning

Use the following five-sentence structure by default when these roles have not already been covered in a discussion:

1. Restate the research problem and give the core judgment directly, without repeating experimental numbers.
2. Interpret what that judgment means within the field.
3. Explain its relationship to previous findings; if results differ, give a supported explanation or identify the cause as unresolved rather than inventing one.
4. State the material limitation concisely.
5. Identify the next research direction that follows from it.

If the discussion already covers a role, do not repeat that content merely to reach five sentences. Retain the central answer and significance, and use a shorter conclusion. Do not introduce new results or claims here.

## Overall voice: present the contribution with confidence

Apply the user's **product-launch principle**: lead with the problem solved, the mechanism, the supported advantages, and why they matter. Write direct, connected academic English. Use precise verbs and concrete claims rather than inflated adjectives, repeated hedging, or procedural narration.

Avoid defensive writing and recurring experiment-report prose. Keep internal process vocabulary out of manuscripts, including terms such as “freeze,” “audit,” “probe,” “hash,” and “gate” when used as workflow labels, and equivalent operational language. If the scientific subject itself requires a conflicting term, ask about that conflict instead of silently changing the technical meaning.

Positive presentation must remain accurate. Do not exaggerate novelty, universality, causality, or superiority. State essential conditions near the claim they qualify; concentrate interpretive limitations in the user-approved discussion or conclusion rather than repeating them throughout the paper. Correct straightforward numerical or factual mistakes within the authorized edit and explain the correction; ask before changing the paper's larger contribution positioning or removing substantive material. A confident tone never licenses fabricated evidence or misleading omission.

## Final pass and delivery

Check that the abstract's result answers its problem, the introduction's gap leads to the method, the overview matches the modules and equations, and every experimental claim supports a contribution. Check sources, values, metric directions, captions, and rendered visuals actually produced. Remove repeated narration and unrequested edits within the authorized scope.

Deliver the requested text or files. Briefly explain meaningful edits and their purpose outside the manuscript. State what was checked and any remaining factual gaps or user decisions without inserting process notes into the paper. If a dependency remains unresolved, identify exactly which part is incomplete and continue the rest of the authorized work.
