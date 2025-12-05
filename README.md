# 🏭 铝型材智能报价系统 (Aluminum Profile Quotation System)

> 一个基于微信小程序的高颜值、智能化 B2B 铝型材报价工具。
> A Glassmorphism style WeChat Mini Program for Aluminum Profile B2B pricing.

![Version](https://img.shields.io/badge/Version-1.5.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-WeChat_Mini_Program-green.svg)
![License](https://img.shields.io/badge/License-MIT-orange.svg)

## 📖 项目简介 (Introduction)

本项目是一个专为铝型材行业销售人员打造的移动端报价工具。旨在解决传统报价过程中“计算繁琐、公式复杂、缺乏记录”的痛点。

不同于传统的工业软件，本项目采用了 **玻璃拟态 (Glassmorphism)** 设计语言，结合 **3D 翻转交互**，在保证专业计算精度的同时，提供了极佳的用户体验和视觉享受。

## ✨ 核心功能 (Features)

### 1. 🧮 智能双模报价
- **按吨报价**：支持标准的铝锭基价 + 加工费 + 附加费计算逻辑。
- **按支报价**：自动换算米重与长度，支持“元/支”维度的精确报价。
- **税务计算**：内置不含税、中联、中畅等多种税率快捷切换。

### 2. 📐 工程师模式 (Engineer Mode)
- **3D 翻转交互**：点击工具栏齿轮图标，卡片 3D 翻转至背面。
- **几何米重计算**：内置圆管、方管、椭圆管、实心条、实心棒的理论米重计算公式。
- **一键应用**：计算结果可直接应用至正面的报价单中。

### 3. 🎨 极致 UI/UX
- **玻璃拟态风格**：全磨砂玻璃质感，适配 iOS 风格色彩体系。
- **动态交互**：数字滚动增加动画、卡片翻转特效。
- **防抖优化**：强制 GPU 渲染，解决 3D 变换时的字体抖动问题 (v2.0 CSS)。

### 4. 📋 商务辅助
- **一键复制**：生成符合商务规范的文本格式报价单，包含详细计算公式。
- **自定义工艺**：支持手动输入特殊表面处理工艺。

## 🛠 技术栈 (Tech Stack)

- **框架**：微信小程序原生 (Native WXML/WXSS/JS)
- **样式**：CSS3 (Flexbox, Transform 3D, Backdrop-filter)
- **逻辑**：ES6+, MVVM 数据绑定

## 📂 项目结构 (Structure)

```text
Aluminum-Quote/
├── pages/
│   └── index/
│       ├── index.wxml       # 页面结构 (v1.0)
│       ├── index.wxss       # 样式表 (v2.0 - 含防抖与GPU加速)
│       ├── index.js         # 逻辑层 (含数字滚动与计算核心)
│       └── index.json       # 页面配置
├── images/                  # 图标资源
├── app.js                   # 全局逻辑
├── app.json                 # 全局配置
└── README.md                # 项目说明文档
