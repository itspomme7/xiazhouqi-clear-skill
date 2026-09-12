# Xiazhouqi Clear Skill

> **Xiazhouqi Clear｜下周七·清透** — 为信息密集型页面整理的一套清透、克制、耐看、移动端优先的个人 Web 设计规范

[English](./README.md) · [完整 Skill](./SKILL.md) · [更新记录](./CHANGELOG.md)

属于 **[Xiazhouqi](https://xiazhouqi7.com)** 设计体系。

## 一句话定义

> **不全抄苹果，但保留苹果的克制；不堆满颜色，但允许颜色承担信息层级**

执行层原则：

> **结构负责秩序，字重负责重点，阴影负责层级，颜色负责分类**

Clear 不是纯黑白灰，也不是 Apple 官网复刻。它保留 Apple 式界面的克制、留白和低噪音骨架，再用低饱和语义色、信息分组、字重和阴影建立自己的信息层级。

## 适用页面

- 邮箱档案
- Apple ID / 外区账号档案
- 银行卡档案
- 固定支出 / 财务规划
- 私人档案馆总入口
- 下载入口页 / 工具页
- 账号管理页
- 数据清单
- 需要长期维护的单文件 HTML

如果页面更偏生活、叙事、纪念、奶杏和温柔文学感，优先使用 `Xiazhouqi Warm｜下周七·暖杏`。

## Clear 的核心

1. **先分组，再美化**：先判断平台、地区、用途、优先级、当前/历史，再决定组件和颜色
2. **颜色必须有含义**：邮箱按平台、Apple ID 按地区、银行卡按资金用途、消费规划按资金类别
3. **中性骨架高于主色**：body、Header、Section、Card 默认白灰；颜色只做局部分类信号，禁止整页同色化
4. **层级不靠一个手段完成**：结构管关系、字重管重点、阴影管视觉等级、颜色管分类
5. **Core / Normal / Quiet 三档**：核心内容更稳，普通内容正常，历史/备用内容退后
6. **内容优先**：改风格默认不改数据；要求“按最新标准”时，优先使用用户最新明确确认的信息
7. **短文案克制**：标题、副标题、标签、页尾短句默认不加句号；不为了设计感硬加解释性文案
8. **手机真实使用优先**：390px 与 360–380px 都要可用，长邮箱、长卡号、多标签不能横向溢出
9. **交互要可靠**：复制按钮可以小而淡，但点击必须稳定；输入框避免 iPhone 自动放大
10. **本地 HTML 兼容是硬规则**：核心正文不要放在 iframe / srcdoc；关键进入、切换、正文显示不要只依赖脆弱 JavaScript
11. **代码最终要干净**：旧文件补丁过多时优先重构，不继续无限叠 `!important` 和 v1/v2/v3 CSS patch

## 当前版本

**v1.2.0 — 2026-09-12**

这一版以总档案馆中已经确认的邮箱和消费支出规划为最终样板，重点补齐了：

- 中性白灰骨架必须高于页面主色
- 禁止全页背景、卡片、标签和控件同时套成蓝色
- 每个视觉层级只使用 1–2 种颜色载体
- 父子容器避免重复叠加 accent wash
- 邮箱 / 消费规划最终样板优先于抽象规则
- 新增日常任务、年度计划和历史记录页模式

## 仓库结构

```text
.
├─ README.md
├─ README.zh-CN.md
├─ SKILL.md
├─ CHANGELOG.md
├─ VERSION
├─ tokens.css
├─ reference.html
├─ LICENSE
├─ .gitignore
├─ references/
│  ├─ hierarchy-and-color.md
│  ├─ canonical-visual-patterns.md
│  ├─ content-patterns.md
│  ├─ mobile-and-compatibility.md
│  ├─ copy-and-content.md
│  └─ maintenance-and-checklist.md
└─ examples/
   ├─ README.md
   └─ clear-information-cards.html
```

## 触发词

`xiazhouqi-clear` · `Xiazhouqi Clear` · `下周七·清透` · `清透风格` · `苹果感但不要照抄苹果` · `信息多但要耐看`

## Xiazhouqi 体系

- **Clear** — 清透、克制、信息优先的界面设计
- **[Warm](https://github.com/xiazhouqi7/xiazhouqi-warm-skill)** — 温暖、柔和、偏个人化的视觉设计
- **[Photography](https://github.com/xiazhouqi7/xiazhouqi-photography-skill)** — 摄影、调色与视觉叙事

## License

MIT
