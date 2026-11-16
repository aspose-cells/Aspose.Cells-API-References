---
title: "FindOptions 类"
linktitle: "FindOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FindOptions 类。封装了在 Go 中表示 findoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/findoptions/
---

## FindOptions class

表示查找选项。

```go

type FindOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFindOptions](./newfindoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetCaseSensitive](./getcasesensitive/) | 指示搜索的字符串是否区分大小写。 |
| [SetCaseSensitive](./setcasesensitive/) | 指示搜索的字符串是否区分大小写。 |
| [GetLookAtType](./getlookattype/) | 查看类型。 |
| [SetLookAtType](./setlookattype/) | 查看类型。 |
| [GetRange](./getrange/) | 获取和设置搜索范围。 |
| [SetRange](./setrange/) | 设置搜索范围。 |
| [IsRangeSet](./israngeset/) | 指示是否已设置搜索范围。 |
| [GetSearchBackward](./getsearchbackward/) | 是否向后搜索单元格。 |
| [SetSearchBackward](./setsearchbackward/) | 是否向后搜索单元格。 |
| [GetSearchOrderByRows](./getsearchorderbyrows/) | 指示搜索是按行还是按列进行。 |
| [SetSearchOrderByRows](./setsearchorderbyrows/) | 指示搜索是按行还是按列进行。 |
| [GetLookInType](./getlookintype/) | 查找类型。 |
| [SetLookInType](./setlookintype/) | 查找类型。 |
| [GetRegexKey](./getregexkey/) | 指示搜索键是否为正则表达式。如果为 true，搜索键将被视为正则表达式并进行解析。否则，键将按照 MS Excel 的规则进行解析。 |
| [SetRegexKey](./setregexkey/) | 指示搜索键是否为正则表达式。如果为 true，搜索键将被视为正则表达式并进行解析。否则，键将按照 MS Excel 的规则进行解析。 |
| [GetValueTypeSensitive](./getvaluetypesensitive/) | 指示搜索的单元格值类型是否应与搜索键相同。 |
| [SetValueTypeSensitive](./setvaluetypesensitive/) | 指示搜索的单元格值类型是否应与搜索键相同。 |
| [GetStyle](./getstyle/) | 要搜索的格式。 |
| [SetStyle](./setstyle/) | 要搜索的格式。 |
| [GetConvertNumericData](./getconvertnumericdata/) | 获取或设置一个值，指示是否将搜索的字符串值转换为数值数据。 |
| [SetConvertNumericData](./setconvertnumericdata/) | 获取或设置一个值，指示是否将搜索的字符串值转换为数值数据。 |
