# 文件格式规范

## 文件位置

**根目录**: `C:\Users\kezhe\Documents\同步\私人笔记\Obsidians\finance`

**交易文件**: `transactions/YYYY-MM-DD-HHmm-描述.md`

## YAML Frontmatter 格式

```yaml
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
```

## Tag规则（必须4个，必须带单引号）

- `'#finance'` - 系统标记
- `'#txn'` - 交易标记  
- `'#type/支出'` - 类型（支出/收入/转账）
- `'#cat/餐饮'` - 分类（餐饮/日常/项目/资产/其他）

## 字段要求

| 字段 | 要求 | 示例 |
|-----|------|------|
| datetime | YYYY-MM-DD HH:mm | 2026-02-10 14:05 |
| type | 中文：支出/收入/转账 | 支出 |
| amount | 支出为负数 | -10 |
| category | 4选1 | 餐饮 |
| description | 简短描述 | 包子 |
| tags | 4个带单引号的Tag | 见上文 |

## 完整示例

```yaml
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

## 禁止事项

❌ 不要不带单引号（错误：`#finance`）  
❌ 不要英文Tag（错误：`'#type/expense'`）  
❌ 不要双链 `[[...]]`  
❌ 不要新分类  
❌ 不要额外Tag
