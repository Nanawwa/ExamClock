# 考试倒计时

五柳学校考试倒计时工具，适用于教室投影场景。

![License](https://img.shields.io/badge/license-GPL--3.0-blue)

## 功能

- 考试剩余时间大字倒计时
- 进度条可视化
- 全屏投影支持
- 毛玻璃（Glassmorphism）视觉设计
- 风景背景图自动轮换（考试期间暂停）
- 科目快捷选择
- 单文件，双击即用

## 使用

双击打开 `index.html`。

1. 选择或输入科目名称
2. 选择日期、开始时间、考试时长
3. 点击"开始倒计时"
4. 右上角按钮进入全屏

## 替换背景图片

打开 `index.html`，找到脚本中的 `bgImages` 数组，替换为你自己的图片链接即可：

```js
var bgImages = [
  "https://example.com/image1.jpg",
  "https://example.com/image2.jpg",
  // ...
];
```

### 图片要求

- **推荐尺寸**：1920×1080 或更大
- **格式**：JPG / PNG / WebP
- **内容**：风景、自然、建筑等安静的背景图，避免人像
- **数量**：建议 5-15 张，太少会单调，太多加载慢
- **轮换间隔**：默认 30 秒，可修改 `setInterval` 的第二个参数（毫秒）

### 免费图片来源

- [Unsplash](https://unsplash.com) — 免费高清风景图
- [Pexels](https://www.pexels.com) — 免费图片
- [Pixabay](https://pixabay.com) — 免费图片

使用时将图片 URL 末尾的 `?w=1920&q=80` 保留，可控制输出尺寸和质量。

## 技术栈

- 单 HTML 文件，内联 CSS + JS
- 零依赖，无需构建工具
- 双层 DOM 淡入淡出实现背景平滑切换

## 浏览器支持

Chrome 76+ · Firefox 103+ · Safari 14+ · Edge 79+

## 许可证

[GPL-3.0](LICENSE)

## 致谢

本项目基于 [ExamClock](https://github.com/L33Z22L11/ExamClock) 重构，原作者：纸鹿 (L33Z22L11)，野生技协。
