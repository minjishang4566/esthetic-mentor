# Aesthetic Mentor

[English](README.md) | [简体中文](README.zh-CN.md)

一位面向 App 创作者的 AI 审美导师。

Aesthetic Mentor 帮助用户把早期产品想法或已有界面，逐步发展成统一、清晰且可执行的视觉方向。它通过有重点的对话、艺术与设计参考，以及基于证据的界面分析，将模糊的审美意图转化为 Visual DNA。

它的职责是引导，而不是替用户决定。图片不是必需输入，参考资料只是可选的探索入口；Skill 会控制分析范围，避免不必要的研究、长篇输出和 token 浪费。

## 它能做什么

- 在提出完整方向前，确认产品、用户、使用场景、平台、情绪目标和限制条件。
- 帮助用户判断：发展更原创的视觉身份，还是从已有 App 中提取可迁移的设计原则。
- 分析已有 App 时，先定义当前风格，再提出优先改进项。
- 从视觉谱系、色彩关系、形状语法、字体、构图、材料感和情绪张力理解灵感。
- 在需要时提供艺术家、艺术运动、博物馆、家具、编辑设计和 Pinterest 搜索方向。
- 提供三个真正不同的候选方向，并评估 Brand Fit、Color Fit、Shape Fit、UI Fit 和 Personality Fit。
- 将选定方向转译为设计 Token、组件行为、动效、触觉反馈、状态、设计边界和开发交接规范。
- 根据已经确定的 Visual DNA 审查实现截图，不随意推翻已经确认的设计决定。

## 交互原则

- 每次只问一个真正会影响设计结果的问题。
- 使用用户已经提供的信息，不要求重复回答。
- 不规定用户必须提供什么参考图或多少张图片。
- 按照 `视觉证据 -> 感受影响 -> 可迁移原则 -> 下一步选择` 解释判断。
- 普通回复保持简洁，只在用户需要完整分析或定义书时展开。
- 概念尚未完整、Brief 尚未确认时，不提前输出完整设计项目。

## 工作流

1. **理解产品：** 确认用途、用户、场景、平台和期望感受。
2. **选择路径：** 原创视觉身份、已有 App 参考、灵感分析或现有界面诊断。
3. **阅读证据：** 找出反复出现的视觉关系，不急于套用流行风格标签。
4. **提出方向：** Brief 完整后，给出三个差异明确且能实际落地的方向。
5. **逐步收敛：** 一次解决一个颜色、形状、字体、密度或情绪温度问题。
6. **定义系统：** 输出 Visual DNA、Token、组件、动效、状态、边界和交接规则。
7. **检查实现：** 对照选定方向审查截图，指出最值得优先修复的问题。

## 灵活输入

用户可以从自己当前拥有的任何信息开始：

- 一个 App 想法；
- 已有界面或截图；
- 一个链接、艺术家、艺术品、App、物件或设计运动；
- 一种颜色、材料、情绪、描述词或明确不喜欢的东西；
- 完全没有视觉参考。

如果更多视觉证据确实会改善判断，Aesthetic Mentor 可以提供可选搜索关键词，并告诉用户应该观察什么关系。用户仍然可以分享任何自己认为相关的内容，或者完全用文字继续。

## 可以输出什么

根据用户的目标，Skill 可以提供：

- 当前视觉风格定义与优先改进项；
- 精简的 Taste Profile；
- 三个候选审美方向及适配度分析；
- Visual DNA 摘要；
- 颜色角色与使用比例；
- Shape、Typography 与 Icon Grammar；
- 组件、动效、触觉反馈和状态规则；
- Do/Don't 设计边界；
- 完整的 App Design Definition Book 与开发交接规范；
- 基于截图的 Visual DNA 复盘。

## 安装

将仓库克隆到 Codex Skills 目录：

```bash
git clone https://github.com/minjishang4566/esthetic-mentor.git ~/.codex/skills/aesthetic-mentor
```

如果 Skill 没有立即出现，请重新启动或刷新 Codex。

## 使用

显式调用：

```text
$aesthetic-mentor 帮我找到适合这个 App 的视觉方向。
```

也可以自然地开始：

```text
我想做一个宠物健康日记 App，但现在还没有视觉方向。
```

```text
这是我现有 App 的截图。请先定义它现在的风格，再帮助我判断应该延续还是重新创造一个方向。
```

## 文件结构

```text
.
|-- README.md
|-- README.zh-CN.md
|-- SKILL.md
|-- agents/
|   `-- openai.yaml
`-- references/
    |-- concept-readiness.md
    |-- curatorial-guidance.md
    |-- design-definition-template.md
    |-- direction-scorecard.md
    |-- existing-app-path.md
    |-- image-rubric.md
    |-- reference-sourcing.md
    `-- taste-profile-review.md
```

## 边界

Aesthetic Mentor 提取可迁移的视觉原则，不复制在世艺术家、品牌、App 或具有明显识别性的艺术作品。像素级复刻与参考图实现应交由独立的实现工作流完成。
