# Bases查询示例

## 支出查询

```base
filters:
  and:
    - file.hasTag("finance")
    - type == "支出"
properties:
  datetime:
    label: 时间
  amount:
    label: 金额
  category:
    label: 分类
  description:
    label: 描述
sort:
  - property: datetime
    direction: desc
```

## 按分类统计

```base
filters:
  and:
    - file.hasTag("finance")
    - category == "餐饮"
properties:
  datetime:
    label: 时间
  amount:
    label: 金额
  description:
    label: 描述
```
