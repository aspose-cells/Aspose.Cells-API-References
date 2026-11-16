---
title: "AccessCacheOptions 枚举"
linktitle: "AccessCacheOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AccessCacheOptions 枚举。封装在 Go 中表示 accesscacheoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

数据访问的缓存选项。多个选项可以使用 "|" 运算符组合。

```go

type AccessCacheOptions int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [None](./none/) | 对任何数据访问均不使用缓存。 |
| [All](./all/) | 对工作簿中所有类型的数据访问应用所有可能的优化。在优化访问期间，不应更改任何设置和数据。 |
| [PositionAndSize](./positionandsize/) | 对获取对象（例如 Shape）的位置信息和大小应用可能的优化。在优化访问期间，不应更改行高和列宽设置。 |
| [CellsData](./cellsdata/) | 对获取单元格值应用可能的优化。单元格数据（单元格和行的数值及设置）在优化访问期间不应被更改，也不应创建新的 Cell/Row 对象（例如通过 <see cref=\"Cells.this[int, int]\"/>）。 |
| [CellDisplay](./celldisplay/) | 对获取单元格的显示相关结果（<see cref=\"Cell.DisplayStringValue\"/>、<see cref=\"Cell.GetStyle()\"/>、<see cref=\"Cell.GetDisplayStyle()\"/> 等）应用可能的优化。在优化访问期间，不应更改单元格数据和样式相关对象（单元格/行/列样式、列宽等）。 |
| [GetFormula](./getformula/) | 对获取公式应用可能的优化。所有可能影响公式表达式的数据信息和设置（工作表名称、名称文本、表格列等）在优化访问期间不应被更改。 |
| [SetFormula](./setformula/) | 对设置公式应用可能的优化。所有可能影响公式表达式的数据信息和设置（工作表名称、名称文本、表格列等）在优化访问期间不应被更改。 |
| [CalculateFormula](./calculateformula/) | 对计算公式应用可能的优化。单元格数据在优化访问期间不应被更改，也不应创建新的对象（Cell、Row 等）（例如通过 <see cref=\"Cells.this[int, int]\"/>）。 |
| [ConditionalFormatting](./conditionalformatting/) | 对获取条件格式的格式化结果应用可能的优化。所有可能影响条件格式结果的数据信息和设置（条件格式的设置、相关单元格值等）在优化访问期间不应被更改。 |
| [Validation](./validation/) | 对获取验证结果应用可能的优化。所有可能影响验证结果的数据信息和设置（验证的设置、相关单元格值等）在优化访问期间不应被更改。 |
