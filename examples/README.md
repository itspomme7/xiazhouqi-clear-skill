# Examples

这些示例只演示 Xiazhouqi Clear 的信息结构与视觉逻辑，不包含真实个人数据。

## `clear-template.html` — Canonical Reference

这是当前 Xiazhouqi Clear 的**官方全组件视觉基准母版**。

生成或重构网页前，优先读取并观察这份模板，重点学习：

- 冷白 / 浅灰的中性骨架
- 低饱和语义色的使用范围
- Hero、Section、Card 的层级关系
- Core / Normal / Quiet 三档视觉权重
- 数据卡、进度环、进度条
- 信息列表、标签、状态、复制交互
- Input / Select / Textarea / Switch / Tabs
- 任务勾选与完成状态
- Accordion、Timeline、私密入口、空状态、Toast
- 手机端单列与桌面端多列的响应式关系

**不要机械复制示例文案。** 应复用它的视觉语言、比例、间距、层级和组件逻辑，再根据实际内容重新组织页面。

如果抽象文字规则与已经确认的视觉结果出现轻微差异，`clear-template.html` 可作为视觉判断的重要基准；数据、内容安全与明确硬规则仍以 `SKILL.md` 为准。

## `clear-information-cards.html`

用于观察：

- Core / Normal / Quiet 三档视觉权重
- 平台 / 地区 / 用途的低饱和语义色
- 长字符串在手机端的换行
- 小而淡的复制按钮
- 390px 与 360–380px 宽度下的单列布局
- 桌面端根据内容密度扩展到多列

## 使用方式

优先直接双击本地 HTML 测试，再放到浏览器和 GitHub Pages 中测试。

推荐读取顺序：

1. `SKILL.md`
2. `examples/clear-template.html`
3. 任务需要时再读取 `references/`、`tokens.css` 与其他 examples

如果示例与 `SKILL.md` 的数据、安全或明确硬规则冲突，以 `SKILL.md` 和当前版本 `VERSION` 为准。
