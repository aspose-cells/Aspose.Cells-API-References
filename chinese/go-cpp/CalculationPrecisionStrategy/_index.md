---
title: "CalculationPrecisionStrategy 枚举"
linktitle: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CalculationPrecisionStrategy 枚举。封装了在 Go 中表示 calculationprecisionstrategy 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

枚举处理计算精度的策略。由于 IEEE 754 浮点运算的精度问题，一些 \"seemingly simple\" 公式可能无法得到预期结果。例如公式 \"=-0.45+0.43+0.02\"，直接使用 '+' 运算符计算操作数时，结果不是零。针对这种精度问题，某些特殊策略可能会得到预期结果。

```go

type CalculationPrecisionStrategy int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [None](./none/) | 在计算时未应用任何策略。计算时仅使用原始 double 值作为操作数并直接返回结果。对性能最有效，适用于大多数情况。 |
| [Round](./round/) | 根据有效数字对计算结果进行四舍五入。 |
| [Decimal](./decimal/) | 在可能的情况下使用 decimal 作为操作数。对性能最不高效。 |
