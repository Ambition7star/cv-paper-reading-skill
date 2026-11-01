# cv-paper-reading-skill

> A structured, top-conference-grade paper reading workflow for Computer Vision & AI researchers — packed as an installable Agent Skill.

A deep, rigorous, reproducible **paper-reading protocol** for CV/AI research, distilled from practical experience on RGB-T / multi-modal object detection, Mamba architectures, and low-altitude UAV scenes. It turns a single paper into: a from-zero full reading → an experiment plan → a writing-teardown → a reusable writing template.

## 🎯 Positioning

- **Target domain**: Computer Vision & AI (object detection, multi-modal fusion, RGB-T/RGBT, Mamba, low-altitude UAV).
- **Audience**: graduate students and researchers who read papers to reproduce, review, and write their own.
- **Philosophy**: evidence over marketing — judge what a paper *actually* proved, never just restate its claims.

## 📦 What it contains

```
cv-paper-reading-skill/
├── paper-reading/            # the installable Skill (folder)
│   ├── SKILL.md              # workflow decision tree + core principles + output contract
│   └── references/
│       ├── part1-deep-reading.md      # 13-aspect full paper reading (method, formulas, figures, experiments, ablations, evidence boundary)
│       └── part2-writing-analysis.md  # narrative logic, section-by-section teardown, evidence chain, writing checklist
└── README.md
```

### Part 1 — From-zero full reading (13 aspects)
Positioning · Motivation · Theory (every formula explained) · Architecture & data flow (tensor shapes) · Core mechanism · Figures & tables · Experiments (FLOPs/params/fairness) · Ablations · Evidence boundary · Limitations & failure cases · **Ideas for your own RGB-T research** · Experiment objectification (reproducible plan) · Final research judgment (with a ready-to-use group-meeting summary).

### Part 2 — Writing & logic teardown (9 aspects)
Full causal chain · Chapter-by-chapter structure · Argumentation role of each section · Figure/table/equation function · Evidence-chain closure · Reverse-infer the actual research workload · Writing strengths & weaknesses · Transferable paper-writing template · Complete self-check checklist.

## 🚀 How to use

Install the `paper-reading/` folder as a Skill in your agent environment, then say e.g.:

> "精读这篇论文" / "Deep-read this paper" / "帮我做组会汇报" / "分析这篇论文怎么写出来的"

It will output the full reading **first in chat**, then generate two Markdown files:
- `论文名_完整精读与实验假设.md`
- `论文名_论文逻辑框架与科研写作分析.md`

## ✨ Why it stands out

- **Fixed contract**: complete output, never trimmed, no mid-way "shall I continue?" interruptions.
- **Three-layer rigor**: paper's own claims / what follows from the paper / my critical judgment — clearly separated.
- **Repro-friendly**: every paper is turned into a concrete, ablatable experiment plan.
- **RGB-T oriented**: explicitly connects to RGB-T/RGBT detection, modal degradation, misalignment, small objects, Mamba — with testable research hypotheses.

## 📌 License

MIT
