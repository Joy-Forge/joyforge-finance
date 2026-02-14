# 路径配置指南

## 默认路径

技能使用以下默认路径结构：

```
~/Documents/Obsidians/finance/
├── transactions/          # 交易记录目录
└── analytics/             # 分析报告目录（自动生成）
```

## 自定义路径

### 方法1：对话中指定（推荐）

在 OpenClaw 中直接说：

```
设置记账目录为 D:\MyFinance\transactions
```

或执行报表脚本时指定：

```powershell
.\Generate-FinanceReport.ps1 -TransactionsPath "D:\\MyFinance\\transactions"
```

### 方法2：修改脚本默认值

编辑 `Generate-FinanceReport.ps1` 第12行：

```powershell
$TransactionsPath = Join-Path $docs "YOUR_CUSTOM_PATH_HERE"
```

### 方法3：设置环境变量

```powershell
$env:JOYFORGE_FINANCE_PATH = "D:\\MyFinance\\transactions"
```

## 目录结构要求

无论路径在哪里，都需要保持以下结构：

```
your-finance-folder/
├── transactions/          # 必须：存放交易 .md 文件
└── analytics/             # 可选：报表自动生成到这里
```

## 示例配置

### Windows
```powershell
D:\Documents\finance\transactions
```

### macOS/Linux
```bash
~/Documents/finance/transactions
```

### iCloud/OneDrive 同步
```
iCloudDrive/Obsidians/finance/transactions
```
