---
title: "LookInType 枚举"
linktitle: "LookInType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LookInType 枚举。封装了在 Go 中表示 lookintype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/lookintype/
---

## LookInType Enum

表示 LookIn 类型。

```go

type LookInType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Formulas](./formulas/) | 如果单元格是公式，则从公式(<see cref="Cell.Formula"/>)中查找目标对象；否则从单元格的原始值中查找（与 <see cref="OriginalValues"/> 相同）。 |
| [Values](./values/) | 从单元格的原始值(<see cref="Cell.Value"/>)和格式化值(<see cref="Cell.StringValue"/>)中查找对象。 |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | 忽略公式单元格。对于非公式单元格，行为与 <see cref="Values"/> 相同。 |
| [Comments](./comments/) | 仅从单元格的批注中查找对象。忽略没有批注的单元格。 |
| [OnlyFormulas](./onlyformulas/) | 忽略非公式单元格。对于公式单元格，从公式(<see cref="Cell.Formula"/>)中查找目标对象。 |
| [OriginalValues](./originalvalues/) | 仅从单元格的原始值中查找对象。 |
| [FormattedValues](./formattedvalues/) | 仅从单元格的格式化值(<see cref="Cell.StringValue"/>)中查找对象。 |
