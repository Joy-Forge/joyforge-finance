---
name: joyforge-finance
version: 1.1.0
description: JoyForge极简记账 - 检测到消费关键词时自动记录交易
author: 小心心
for: 走正路
organization: JoyForge
tags: [finance, accounting]
---

# JoyForge 极简记账

**触发词**：买了、花了、支出、支付、消费、拼多多、淘宝、京东、美团

## 核心规则

### 1. 文件位置
`C:\Users\kezhe\Documents\同步\私人笔记\Obsidians\finance\transactions\YYYY-MM-DD-HHmm-描述.md`

### 2. 分类（4选1）
- **餐饮**：包子、面条、奶茶、水果、零食
- **日常**：纸巾、水电、交通、衣服
- **项目**：AI、服务器、课程、软件
- **资产**：买房、买车、大额投资

### 3. 必须执行的流程
1. 检测到消费 → 立即记账
2. 提取：金额、商品、渠道、时间
3. 自动分类（4选1）
4. 创建交易文件（4个带引号的Tag）
5. 回复："✅ 已记账：商品 ¥金额（分类）"

**详细规范**：见 `references/file-format.md`  
**AI识别规则**：见 `references/ai-rules.md`  
**Bases查询**：见 `references/bases-queries.md`

---
维护者: 小心心 | JoyForge
