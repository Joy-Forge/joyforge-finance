# JoyForge Finance

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Compatible-blue)](https://openclaw.ai)

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
# 手动克隆到 OpenClaw 技能目录
git clone https://github.com/Joy-Forge/joyforge-finance.git
cd joyforge-finance
# 复制到 OpenClaw skills 目录（根据你的安装位置调整）
```

### 2. 配置

**默认路径结构**（可在对话中自定义）：

```
~/Documents/finance/           # 财务根目录
├── transactions/              # 交易记录（必须）
│   └── YYYY-MM-DD-HHmm-描述.md
└── analytics/                 # 分析报告（自动生成）
    └── YYYY-MM-report.md
```

**自定义路径**：
在 OpenClaw 对话中直接说：
```
设置记账目录为 D:\MyFinance\transactions
```

详细配置见 [path-configuration.md](references/path-configuration.md)

### 3. 开始记账

对 AI 说：
- "今天买咖啡花了 25 元"
- "拼多多买了手机壳 9.9"
- "支出 500，类别项目，买服务器"

## 📁 文件结构

交易文件命名格式：
```
transactions/YYYY-MM-DD-HHmm-描述.md
```

示例：
- `2026-02-10-0830-早餐包子.md`
- `2026-02-10-1200-午餐面条.md`

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

## 📚 文档

- [文件格式规范](references/file-format.md)
- [AI 识别规则](references/ai-rules.md)
- [路径配置指南](references/path-configuration.md)
- [Dataview 查询](references/bases-queries.md)

## 🔗 相关项目

- [OpenClaw](https://openclaw.ai) - AI 助手平台

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

---

**JoyForge** - 创造喜悦的技术工坊
