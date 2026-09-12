# Mobile & Compatibility

## 1. 目标环境

优先保证：

- iPhone Safari
- iPhone 文件 / 本地 HTML 预览
- 390px 常见宽度
- 360–380px 更窄设备
- 桌面 Chrome / Edge

手机真实可用性优先于桌面 Demo 效果。

## 2. 防横向溢出

```css
* { box-sizing: border-box; }

html, body {
  max-width: 100%;
  overflow-x: hidden;
}

.card,
.row,
.value,
.title {
  min-width: 0;
}

.breakable {
  overflow-wrap: anywhere;
}
```

Grid（网格）优先：

```css
grid-template-columns: minmax(0,1fr);
```

避免会强行撑宽页面的固定宽度。

## 3. 输入框防 iOS 自动放大

```css
@supports (-webkit-touch-callout:none) {
  input,
  textarea,
  select,
  button {
    font-size: 16px;
  }
}
```

## 4. 复制按钮

按钮视觉可以 20–24px，但必须稳定点击。

```css
.card::before,
.card::after {
  pointer-events: none;
}

.copy-btn {
  position: relative;
  z-index: 5;
  pointer-events: auto;
  touch-action: manipulation;
}
```

不要让整张卡的 click（点击）事件抢走按钮事件。

## 5. 密码 / 进入机制

对于单文件私人档案，如果只是轻量访问门槛：

- 可以用 `:target`
- 可以用 checkbox + `:checked`
- 兼容环境可用 `:has()`
- JavaScript 作为增强，不作为唯一核心路径

注意：前端单文件密码**不等于加密**，HTML 源码里的数据仍可被读取。

## 6. 核心内容不要放 iframe / srcdoc

iPhone 本地预览可能出现：外框正常、标题正常、正文整块空白。

核心正文必须直接存在当前 DOM（文档对象模型）中。

聚合页可使用 radio / checkbox / `:checked` / `:target` / CSS selector 切换模块。

## 7. JavaScript 降级

JS 适合增强：

- 复制
- Toast（轻提示）
- 小动画
- 非关键交互

关键目标：

> JS 失败时，页面仍能读、能进、能找核心内容

## 8. 最终手机检查

- 390px 无横向滚动
- 360–380px 可使用
- 长邮箱可换行
- 长卡号不撑破卡片
- 多标签不互挤
- 复制按钮可点击
- 输入密码后可以进入
- 输入框不触发 iPhone 页面放大
- 返回目录 / 切换入口可用
