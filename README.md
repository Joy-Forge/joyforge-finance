# JoyForge Finance

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Skill-blue)](https://openclaw.ai)

> 极简 AI 记账系统 - 说句话就能记账，自动生成财务分析

## ✨ 特性

- 🎤 **语音记账** - "买了包子 3 块钱" → 自动记录
- 🏷️ **智能分类** - 餐饮/日常/项目/资产 自动归类
- 📊 **自动报表** - 月度/年度财务分析一键生成
- 🔒 **本地存储** - 数据完全私有，Markdown 格式
- 🆓 **完全免费** - 零成本搭建个人财务系统

## 🚀 快速开始

### 1. 安装

```bash
# 通过 ClawHub 安装（推荐）
npx clawhub install joyforge-finance

# 或手动克隆
git clone https://github.com/Joy-Forge/joyforge-finance.git
```

### 2. 配置

在 OpenClaw 中激活技能，设置你的记账目录：

```yaml
# 默认路径
~/Documents/同步/私人笔记/Obsidians/finance/transactions
```

### 3. 开始记账

对 AI 说：
- "今天买咖啡花了 25 元"
- "拼多多买了手机壳 9.9"
- "支出 500，类别项目，买服务器"

## 📁 文件结构

```
finance/
├── transactions/          # 交易记录
│   ├── 2026-02-10-0830-早餐包子.md
│   ├── 2026-02-10-1200-午餐面条.md
│   └── ...
└── analytics/             # 分析报告（自动生成）
    ├── 2026-01-report.md
    └── 2026-02-report.md
```

## 📝 交易文件格式

```markdown
---
datetime: 2026-02-10 14:05
type: 支出
amount: -10
category: 餐饮
description: 包子
tags:
  - '#finance'
  - '#txn'
  - '#type/支出'
  - '#cat/餐饮'
---

# 包子

- 时间: 2026-02-10 14:05
- 金额: 10元
- 分类: 餐饮
```

## 🔗 相关项目

- [joyforge-finance-analytics](https://github.com/JoyForge/joyforge-finance-analytics) - 财务分析报表
- [OpenClaw](https://openclaw.ai) - AI 助手平台

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 💝 致谢

感谢走正路的产品反馈和小心心的技术实现 ❤️

---

**JoyForge** - 创造喜悦的技术工坊
