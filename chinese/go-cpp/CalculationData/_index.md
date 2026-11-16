---
title: "CalculationData 类"
linktitle: "CalculationData"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CalculationData 类。封装在 Go 中表示 calculationdata 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/calculationdata/
---

## CalculationData class

表示计算函数时所需的数据，例如函数名称、参数等。

```go

type CalculationData struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetCalculatedValue](./getcalculatedvalue/) | 获取或设置此函数的计算值。 |
| [SetCalculatedValue](./setcalculatedvalue/) | 获取或设置此函数的计算值。 |
| [GetWorkbook](./getworkbook/) | 获取函数所在的 Workbook 对象。 |
| [GetWorksheet](./getworksheet/) | 获取函数所在的 Worksheet 对象。 |
| [GetCellRow](./getcellrow/) | 获取函数所在单元格的行索引。 |
| [GetCellColumn](./getcellcolumn/) | 获取函数所在单元格的列索引。 |
| [GetCell](./getcell/) | 获取函数所在的 Cell 对象。 |
| [GetFunctionName](./getfunctionname/) | 获取要计算的函数名称。 |
| [GetParamCount](./getparamcount/) | 获取参数的计数 |
| [GetParamValue](./getparamvalue/) | 获取给定索引处参数的表示值对象。 |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | 获取给定索引处参数的值（们）。如果参数是需要计算的某种表达式，则将在数组模式下进行计算。 |
| [GetParamText](./getparamtext/) | 获取给定索引处参数的文字文本。 |
