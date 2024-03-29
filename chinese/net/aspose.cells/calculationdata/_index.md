---
title: CalculationData
second_title: Aspose.Cells for .NET API 参考
description: 表示计算一个函数时需要的数据如函数名参数等
type: docs
weight: 200
url: /zh/net/aspose.cells/calculationdata/
---
## CalculationData class

表示计算一个函数时需要的数据，如函数名、参数等。

```csharp
public class CalculationData
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue) { get; set; } | 获取或设置此函数的计算值。 |
| [Cell](../../aspose.cells/calculationdata/cell) { get; } | 获取函数所在的Cell对象。 |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn) { get; } | 获取函数所在单元格的列索引。 |
| [CellRow](../../aspose.cells/calculationdata/cellrow) { get; } | 获取函数所在单元格的行索引。 |
| [FunctionName](../../aspose.cells/calculationdata/functionname) { get; } | 获取要计算的函数名 |
| [ParamCount](../../aspose.cells/calculationdata/paramcount) { get; } | 获取参数的计数 |
| [Workbook](../../aspose.cells/calculationdata/workbook) { get; } | 获取函数所在的Workbook对象。 |
| [Worksheet](../../aspose.cells/calculationdata/worksheet) { get; } | 获取函数所在的Worksheet对象。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext)(int) | 获取给定索引处参数的文字文本。 |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue)(int) | 获取给定索引处参数的表示值对象。 |

### 评论

该类提供的所有对象仅用于“读取”目的。 用户在公式计算过程中不应更改工作簿中的任何数据， 否则可能会导致意外结果或异常。

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
