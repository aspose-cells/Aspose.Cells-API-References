---
title: "CalculationOptions 类"
linktitle: "CalculationOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CalculationOptions 类。封装在 Go 中表示 calculationoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/calculationoptions/
---

## CalculationOptions class

表示计算选项。

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetIgnoreError](./getignoreerror/) | 指示在计算公式时遇到的错误是否应被忽略。错误可能是不支持的函数、外部链接等。默认值为 true。 |
| [SetIgnoreError](./setignoreerror/) | 指示在计算公式时遇到的错误是否应被忽略。错误可能是不支持的函数、外部链接等。默认值为 true。 |
| [GetRecursive](./getrecursive/) | 指示在计算一个单元格且它依赖其他单元格时，是否递归计算其依赖单元格。默认值为 true。 |
| [SetRecursive](./setrecursive/) | 指示在计算一个单元格且它依赖其他单元格时，是否递归计算其依赖单元格。默认值为 true。 |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | 指示用户是否已明确指定在计算指定公式之前刷新动态数组公式的行为。 |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | 指示是否在计算公式之前刷新动态数组公式。 |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | 指示是否在计算公式之前刷新动态数组公式。 |
| [GetCustomEngine](./getcustomengine/) | 用于扩展 Aspose.Cells 默认计算引擎的自定义公式计算引擎。 |
| [SetCustomEngine](./setcustomengine/) | 用于扩展 Aspose.Cells 默认计算引擎的自定义公式计算引擎。 |
| [GetCalcStackSize](./getcalcstacksize/) | 递归计算单元格的堆栈大小。默认值为 200。 |
| [SetCalcStackSize](./setcalcstacksize/) | 递归计算单元格的堆栈大小。默认值为 200。 |
| [GetPrecisionStrategy](./getprecisionstrategy/) | 指定计算精度的处理策略。 |
| [SetPrecisionStrategy](./setprecisionstrategy/) | 指定计算精度的处理策略。 |
| [GetLinkedDataSources](./getlinkeddatasources/) | 指定公式中使用的外部链接的数据源。 |
| [SetLinkedDataSources](./setlinkeddatasources/) | 指定公式中使用的外部链接的数据源。 |
| [GetCharacterEncoding](./getcharacterencoding/) | 指定在计算公式时用于字符编码/解码的编码方式。对于 CHAR、CODE 等函数，计算结果取决于区域设置和环境的默认字符集。通过此属性，用户可以指定这些函数使用的适当编码，以获得预期结果。 |
| [SetCharacterEncoding](./setcharacterencoding/) | 指定在计算公式时用于字符编码/解码的编码方式。对于 CHAR、CODE 等函数，计算结果取决于区域设置和环境的默认字符集。通过此属性，用户可以指定这些函数使用的适当编码，以获得预期结果。 |
