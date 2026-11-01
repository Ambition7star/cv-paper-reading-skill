# CV/AI Paper Reading Skill

> **Read beyond the abstract. Reconstruct the argument.**

[简体中文](README.md)

`paper-reading` is an installable Agent Skill for evidence-led reading, reproduction planning, and writing analysis of Computer Vision and AI papers.

It reconstructs a paper as an auditable argument:

**problem → hypothesis → method/data/system design → evidence → boundary → reproducibility and writing insight**

The workflow supports model and empirical papers, datasets and benchmarks, theory and algorithms, systems and efficiency work, surveys and position papers, foundation models, generative AI, and agents. It is deliberately not tied to any private research domain.

## Why this exists

Paper summaries often paraphrase the abstract, walk through sections, and list generic strengths and weaknesses. CV/AI research usually requires a different level of inspection:

- connect equations and diagrams to data flow, state changes, training, and inference;
- distinguish a new mechanism from gains caused by scale, data, compute, or tuning;
- audit splits, pretraining, evaluation protocols, training budgets, and efficiency measurements;
- map every central claim to a figure, table, ablation, proof, or system measurement;
- turn the work into a minimal reproduction and a testable follow-up plan.

This skill makes those research judgments reusable.

## Why not use a generic or Nature-style workflow?

This is a question of domain fit, not overall quality. Nature Paper Card-style tools can be excellent at source grounding, provenance, and standardized analysis across scientific fields. Their fixed card structures and broad scientific taxonomies, however, are not always the most natural entry point for CV/AI papers.

CV/AI conference papers frequently concentrate their contribution in architecture, algorithms, training recipes, benchmark protocols, ablations, and compute budgets.

Applying one universal template can therefore produce predictable mismatches: forcing module analysis onto dataset or theory papers, translating equations without connecting them to implementation, reporting SOTA numbers without checking comparability, or mixing paper claims with code and secondary sources.

`paper-reading` first identifies the paper type, then selects the right unit of analysis and keeps every evidence source explicit.

## Core capabilities

- Adaptive depth: quick explanation, full reading, reproduction plan, writing teardown, or code audit.
- Paper-type-aware analysis for methods, data, theory, systems, surveys, and foundation-model research.
- Five evidence layers: paper fact, author claim, analytical inference, critical judgment, and external/code evidence.
- Claim–evidence mapping instead of abstract paraphrasing.
- Reproduction planning with controls, variables, metrics, risks, and stopping conditions.
- Reverse engineering of narrative, section roles, figures, and research workload.
- Domain-neutral defaults; transfer analysis is added only when the user supplies a target problem.

## Example prompts

```text
Explain what this paper does, what evidence supports it, and where the conclusion stops.

Deep-read this CVPR paper from first principles, focusing on the architecture, losses, and ablations.

Audit the collection, annotation, splits, bias, and evaluation protocol of this dataset paper.

Turn this paper into a minimal reproduction, core ablations, and mechanism-validation plan.

Analyze how the introduction, claim structure, figures, and experiments were designed to tell the story.

Compare the paper with its official code and keep paper evidence separate from code evidence.
```

## Repository layout

```text
cv-paper-reading-skill/
├── paper-reading/
│   ├── SKILL.md
│   └── references/
│       ├── part1-deep-reading.md
│       └── part2-writing-analysis.md
├── README.md
├── README_EN.md
└── LICENSE
```

Copy the entire [`paper-reading/`](paper-reading/) directory into the skills directory of a compatible agent client. The project is Markdown-only, has no runtime dependency, and does not automatically access, modify, or upload papers or code.

## Author

Created and maintained by [Ambition7star](https://github.com/Ambition7star).

Issues and suggestions based on real failure cases are welcome.

## License

[MIT](LICENSE)
