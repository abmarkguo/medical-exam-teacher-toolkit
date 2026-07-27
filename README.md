# Medical Exam Teacher Toolkit · 医考考题分析讲解工具箱

> 面向**医学院教师**的临床执业医师 / 助理医师资格考试**考题获取 · 精准分析 · 考情归纳 · 讲解教学**一体化工具箱。权威、可追溯、可复用。

[English README ↓](#english-readme)

---

## 这个 Skill 解决什么

医学院教师在教研室集体备课、磨课、真题精析中，需要：
1. **获取最新最有特色的考题**（真题 / 回忆版 / 机构题 / 智能命制题）
2. **精准分析**每道题的考点、认知层次、难度、命题陷阱
3. **总结归纳**考情趋势、分值分布、命题规律
4. **把分析转化为教学**，给学生讲清考题

本 Skill 把以上工作沉淀为可重复、权威、可追溯的流程，并明确区分"真题"与"模拟题"。

## 四大模块（闭环）

| 模块 | 功能 | 关键产出 |
|------|------|----------|
| **A 获取与整理** | 结构化采集任意来源考题 + 元数据标注 | 可追溯题库记录 |
| **B 精准分析** | 考点映射 / 认知层次 / 难度 / 陷阱 / 易错点 | 单题分析报告 |
| **C 考情归纳** | 分值分布 / 题型 / 认知层次 / 年度复盘 | 考情报告 + 年度趋势 |
| **D 讲解教学** | 教案 / 课件大纲 / 讲稿 / 误区分层答疑 | 课堂就绪资产 |

闭环：**教师输入 → A 入库 → B 分析 → C 归纳 → D 讲解 → 学生反馈回流优化题库**

智能命制特色模拟题（Module D 生成）回流入库，补充真题不足。

## 权威性保障

每条结论必须可溯源，优先级：
1. 国家卫健委《医师资格考试大纲（2024年版）》+ 2026 医学人文修订
2. 人卫版指导用书 / 第10版教材
3. 医考中心（NMEC）研究报告与创新应用
4. 中华医学会临床诊疗指南
5. 真题考情分析（机构 / 院校教研，标注出处）

> 无法溯源的官方数据一律标 `【待核实】`；AI 生成题必须标注 `【模拟题 · 非真题】`。

## 文件结构

```
medical-exam-teacher-toolkit/
├── SKILL.md                      # 技能主文件
├── references/                  # 8 份参考文档
│   ├── exam-system-teacher-guide.md       # 医考制度与命题导向（教师视角）
│   ├── question-bank-organization.md      # 题库结构化采集与标注
│   ├── question-analysis-methodology.md   # 精准分析方法论
│   ├── cognitive-level-framework.md       # 认知层次框架（记忆/理解/应用）
│   ├── exam-trend-summary.md              # 考情总结归纳方法
│   ├── ai-question-generation.md          # 趋势驱动智能命题
│   ├── teaching-explanation-aids.md       # 讲解教学辅助
│   └── authoritative-sources.md           # 权威来源与溯源规范
├── templates/                   # 8 份模板
│   ├── question-record-template.md        # 考题采集记录
│   ├── question-analysis-template.md      # 单题精准分析
│   ├── exam-report-template.md            # 考情分析报告
│   ├── annual-review-template.md          # 年度命题趋势复盘
│   ├── ai-generated-question-template.md  # 智能命制题记录
│   ├── teaching-plan-template.md          # 考题讲解教案
│   ├── lecture-outline-template.md        # 课件大纲
│   └── qa-guide-template.md               # 误区分层答疑
├── examples/                    # 4 份示例
│   ├── sample-question-analysis.md         # 单题精准分析示例
│   ├── sample-exam-report.md               # 考情分析报告示例
│   ├── sample-ai-question.md              # 智能命制特色题示例
│   └── sample-teaching-plan.md            # 考题讲解教案示例
└── docs/images/                 # 7 张流程图
    ├── system-overview-en.svg
    ├── question-acquisition-en.svg
    ├── question-analysis-en.svg
    ├── exam-trend-summary-en.svg
    ├── teaching-explanation-en.svg
    ├── ai-generation-en.svg
    └── teacher-workflow-en.svg
```

## 流程图一览

| 图 | 内容 |
|----|------|
| system-overview-en.svg | 系统总览：四模块闭环 |
| question-acquisition-en.svg | 模块A：获取与整理流程 |
| question-analysis-en.svg | 模块B：五维精准分析 |
| exam-trend-summary-en.svg | 模块C：考情归纳 |
| teaching-explanation-en.svg | 模块D：讲解教学辅助 |
| ai-generation-en.svg | 趋势驱动智能命题 |
| teacher-workflow-en.svg | 教师完整工作流闭环 |

## 适用对象

- 医学院教师、教研室、执医培训负责人
- 需要实现"考教融合""真题思维进课堂"的教学团队

> 若需求来自**学生**备考，请使用配套的 `medical-exam-prep` Skill。

## License

MIT — 见 [LICENSE](LICENSE)。引用请保留出处与溯源标注。

---

## English README

### What this Skill solves

Medical faculty need to **acquire the latest and most distinctive exam questions**, **analyze them precisely**, **summarize exam trends**, and **explain them to students** — all with authority. This Skill operationalizes that into a repeatable, traceable, reusable workflow, and clearly separates real questions from simulated ones.

### Four modules (closed loop)

- **A · Acquisition & Organization** — structured collection + metadata tagging → traceable question records
- **B · Precise Analysis** — exam-point mapping / cognitive level / difficulty / traps / common errors
- **C · Trend Summary** — score distribution / question types / cognitive levels / annual review
- **D · Teaching Aids** — lesson plan / slide outline / lecture script / misconception Q&A

Loop: **input → A → B → C → D → student feedback refines the bank**. AI-generated characteristic questions feed back into A.

### Authoritative grounding

Every claim is traceable: NHC official syllabus → PMPH guidebooks → NMEC research → clinical guidelines → real-question trend analysis. Unsourced official figures are marked `【待核实】`; AI questions are labeled `【模拟题 · 非真题】` (simulated, not real).

See the file map and 7 SVG flowcharts above. Compatible companion: `medical-exam-prep` (for students).
