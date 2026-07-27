---
name: medical-exam-teacher-toolkit
description: |
  A professional toolkit for medical school faculty to ACQUIRE, ANALYZE, SUMMARIZE, and TEACH
  Chinese Clinical Physician Licensing Examination (临床执业医师/助理医师资格考试) questions.
  Helps teachers collect the latest and most distinctive exam questions, perform precise
  question-level analysis (exam-point mapping, cognitive level, difficulty, question traps),
  summarize annual exam trends, and produce teaching materials (lesson plans, slides, lecture
  scripts, misconception Q&A) to explain questions to students. Authoritative — grounded in the
  NHC official syllabus, PMPH guidebooks, NMEC research reports, and real-question trend analysis.
  Trigger when a medical educator asks about: 医考真题分析, 执医考题讲解, 考情分析, 命题趋势,
  教研室集体备课, 考题库建设, 智能命题, 真题精析, exam question analysis, teaching physician
  licensing exam, clinical faculty exam prep tool.
---

# Medical Exam Teacher Toolkit · 医考考题分析讲解工具箱

> 面向医学院教师的临床执业医师 / 助理医师资格考试**考题获取 · 精准分析 · 考情归纳 · 讲解教学**一体化工具箱。

This skill turns a medical educator's exam-related work into a repeatable, authoritative workflow.
It is built for **faculty**, not students: the goal is to help teachers *understand the exam*,
*organize questions*, *analyze them precisely*, *summarize trends*, and *explain them to students*
with materials they can drop into a lesson.

---

## 1. When to use this skill

Activate this skill when a user (medical faculty / teaching-research office / exam-prep lead) asks to:

- **Acquire & organize** the latest or most distinctive exam questions (真题 / 回忆版 / 机构题 / AI generated)
- **Analyze** a specific question precisely: which exam point, which cognitive level, what difficulty, what trap
- **Summarize** exam trends: annual review, score distribution, newly added points, proposition patterns
- **Teach** a question: build a lesson plan, slide outline, lecture script, or misconception Q&A
- **Generate** characteristic simulation questions driven by syllabus + trend + cognitive-level weighting
- **Build** a traceable departmental question bank with consistent metadata

If the request is from a *student* wanting to study, route to the companion `medical-exam-prep` skill.

---

## 2. Four core modules

The skill is organized as four modules that form a closed loop. Each module has a reference
guide, a fill-in template, and worked examples.

### Module A — Question Acquisition & Organization (考题获取与整理)
Structured collection of questions from any source (real / recall / institution / AI) with
consistent metadata so every question is **traceable** and **reusable**.

- Sources: official syllabus-driven, real-question recall versions, training-institution banks,
  AI-generated characteristic questions (Module D).
- Metadata schema: year, category (执业/助理), stage (技能/综合), unit, question type (A1/A2/A3/A4/B1),
  system, disease, exam point, cognitive level, source, confidence.
- Output: a normalized question record ready for analysis. See `templates/question-record-template.md`.

### Module B — Precise Question Analysis (考题精准分析)
For a single question or a batch, produce a precise analysis report.

- **Exam-point mapping** (考点映射): map to NHC syllabus clause + PMPH textbook chapter.
- **Cognitive level** (认知层次): 记忆 / 理解 / 应用 (Bloom-aligned, three-tier for physician exam).
- **Difficulty** (难度): easy / medium / hard, with rationale.
- **Question traps** (命题陷阱): distractors, misleading wording, cross-system interference.
- **Common errors** (易错点): where students typically fail.
- Output: `templates/question-analysis-template.md`.

### Module C — Exam Trend Summary (考情总结归纳)
Aggregate questions into exam-level insight.

- Score distribution by system / unit / cognitive level.
- Year-over-year change: which points rose, which fell, what was newly added.
- Proposition patterns (命题规律): case-based drift, clinical-reasoning emphasis, "application" weighting.
- Output: `templates/exam-report-template.md` and `templates/annual-review-template.md`.

### Module D — Teaching Explanation Aids (考题讲解教学辅助)
Convert analysis into classroom-ready teaching assets.

- Lesson plan (教案): 考点—知识点—考题 trinity, progressive "organize points → explain question".
- Slide outline (课件大纲): three-stage 章节考点清单 + 典型真题拆解 + 课后专项练测.
- Lecture script (讲稿): teacher-facing narration with student-misconception callouts.
- Misconception Q&A (误区分层答疑): tiered answers for weak / medium / strong students.
- Output: `templates/teaching-plan-template.md`, `templates/lecture-outline-template.md`,
  `templates/qa-guide-template.md`.
- AI-generated characteristic questions feed Modules A→B→C→D. See `references/ai-question-generation.md`.

---

## 3. Authoritative grounding (always cite)

Every output MUST be traceable. Prefer, in order:

1. **National Health Commission (NHC) official syllabus** — 《医师资格考试大纲（2024年版）》+ 2026 医学人文修订.
2. **People's Medical Publishing House (PMPH / 人卫版)** 指导用书 / 第10版教材.
3. **National Medical Examination Center (NMEC / 医考中心)** 研究报告与创新应用（智能命题、病例库、影像题库、自动组卷）.
4. **Chinese Medical Association clinical practice guidelines** 临床诊疗指南.
5. **Real-question trend analysis** from reputable training institutions / faculty research.

When a claim cannot be sourced, mark it `【待核实】` and never present it as official fact.
Do **not** fabricate exact scores, official statistics, or unpublished exam content.

---

## 4. Standard workflow (the closed loop)

```
Teacher input (questions / syllabus / trend need)
        │
        ▼
[A] Acquire & organize  ──► normalized question records (traceable)
        │
        ▼
[B] Analyze precisely    ──► per-question analysis (point/cognitive/difficulty/trap)
        │
        ▼
[C] Summarize trends      ──► exam report / annual review (distribution & patterns)
        │
        ▼
[D] Teach & explain       ──► lesson plan / slides / script / misconception Q&A
        │
        ▼
[Feedback] student outcomes ──► refine question bank & analysis  (loop)
```

The seven SVG flowcharts in `docs/images/` visualize each stage. Start with
`docs/images/system-overview-en.svg` and `docs/images/teacher-workflow-en.svg`.

---

## 5. File map

```
medical-exam-teacher-toolkit/
├── SKILL.md
├── references/
│   ├── exam-system-teacher-guide.md      # Exam system & proposition orientation (faculty view)
│   ├── question-bank-organization.md     # Structured collection & metadata schema
│   ├── question-analysis-methodology.md  # Precise analysis methodology
│   ├── cognitive-level-framework.md      # Memory/Understanding/Application framework
│   ├── exam-trend-summary.md             # Trend summary & annual review method
│   ├── ai-question-generation.md         # Trend-driven characteristic question generation
│   ├── teaching-explanation-aids.md      # Lesson plan / slide / script / Q&A guides
│   └── authoritative-sources.md          # Source hierarchy & citation rules
├── templates/
│   ├── question-record-template.md       # Question acquisition record
│   ├── question-analysis-template.md     # Single-question precise analysis
│   ├── exam-report-template.md           # Exam-level report
│   ├── annual-review-template.md         # Annual proposition trend review
│   ├── ai-generated-question-template.md # AI-generated question record
│   ├── teaching-plan-template.md         # Teaching plan (教案)
│   ├── lecture-outline-template.md       # Slide outline (课件大纲)
│   └── qa-guide-template.md              # Misconception Q&A guide
├── examples/
│   ├── sample-question-analysis.md        # Worked single-question analysis
│   ├── sample-exam-report.md              # Worked exam report
│   ├── sample-ai-question.md             # Worked AI-generated characteristic question
│   └── sample-teaching-plan.md            # Worked teaching plan
└── docs/images/                          # 7 SVG flowcharts (see README)
```

---

## 6. Operating rules

- **Traceability first.** Never output a question or claim without a source label.
- **Faculty lens.** Frame everything for teaching, not just answering.
- **No fabrication.** If you do not know an official figure, say so and mark `【待核实】`.
- **Trend-aware.** Reference the 2025/2026 shifts: more case-based, more application-level,
  AI-assisted proposition, "cross-type no-back" CBT behavior.
- **Reusable output.** Always deliver in a template format the teacher can store and reuse.
