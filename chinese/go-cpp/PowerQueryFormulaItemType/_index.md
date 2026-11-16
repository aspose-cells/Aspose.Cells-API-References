---
title: "PowerQueryFormulaItemType 枚举"
linktitle: "PowerQueryFormulaItemType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PowerQueryFormulaItemType 枚举。封装了在 Go 中表示 powerqueryformulaitemtype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/powerqueryformulaitemtype/
---

## PowerQueryFormulaItemType Enum

表示 Power Query 公式项的类型。

```go

type PowerQueryFormulaItemType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Unknown](./unknown/) | 未知或默认类型。 |
| [Function](./function/) | 该项是函数 (contains => arrow)。 |
| [Parameter](./parameter/) | 该项是参数。 |
| [List](./list/) | 该项是列表 (starts with {)。 |
| [Literal](./literal/) | 该项是字面值 (string, number, boolean, null)。 |
