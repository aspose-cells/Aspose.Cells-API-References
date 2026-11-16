---
title: "FormulaParseOptions 类"
linktitle: "FormulaParseOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FormulaParseOptions 类。封装在 Go 中表示 formulaparseoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

表示解析公式时的选项。

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetLocaleDependent](./getlocaledependent/) | 公式是否使用区域设置格式。默认值为 false。 |
| [SetLocaleDependent](./setlocaledependent/) | 公式是否使用区域设置格式。默认值为 false。 |
| [GetR1C1Style](./getr1c1style/) | 公式是否采用 R1C1 引用样式。默认值为 false。 |
| [SetR1C1Style](./setr1c1style/) | 公式是否采用 R1C1 引用样式。默认值为 false。 |
| [GetCheckAddIn](./getcheckaddin/) | 是否在当前工作簿的现有外部链接中检查用户自定义函数的加载项而不使用外部链接。默认值为 true（如果用户自定义函数与现有外部链接中的某个加载项匹配，则将其视为该加载项）。 |
| [SetCheckAddIn](./setcheckaddin/) | 是否在当前工作簿的现有外部链接中检查用户自定义函数的加载项而不使用外部链接。默认值为 true（如果用户自定义函数与现有外部链接中的某个加载项匹配，则将其视为该加载项）。 |
| [GetParse](./getparse/) | 是否解析给定的公式。默认值为 true。如果为 false，则给定的公式字符串将保持原样，直到用户调用其他方法解析它们，或其他操作（如计算公式）需要已解析的公式数据。 |
| [SetParse](./setparse/) | 是否解析给定的公式。默认值为 true。如果为 false，则给定的公式字符串将保持原样，直到用户调用其他方法解析它们，或其他操作（如计算公式）需要已解析的公式数据。 |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | 自定义函数解析的定义。 |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | 自定义函数解析的定义。 |
