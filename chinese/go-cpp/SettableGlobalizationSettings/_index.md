---
title: "SettableGlobalizationSettings 类"
linktitle: "SettableGlobalizationSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SettableGlobalizationSettings 类。封装在 Go 中表示 settableglobalizationsettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

GlobalizationSettings 的实现，支持用户设置/更改预定义文本。

```go

type SettableGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetTotalName](./gettotalname/) | 获取特定函数的完整名称。 |
| [SetTotalName](./settotalname/) | 设置特定函数的完整名称。 |
| [GetGrandTotalName](./getgrandtotalname/) | 获取函数的总计名称。 |
| [SetGrandTotalName](./setgrandtotalname/) | 设置特定函数的总计名称。 |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | 获取由表头组成的表行的类型名称。默认是 "Headers"，因此在公式中 "#Headers" 代表表头。 |
| [SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | 设置由表头组成的表行的类型名称。 |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | 获取由引用表的数据区域组成的表行的类型名称。默认是 "Data"，因此在公式中 "#Data" 代表表的数据区域。 |
| [SetTableRowTypeOfData](./settablerowtypeofdata/) | 设置由引用表的数据区域组成的表行的类型名称。 |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | 获取引用表中所有行组成的表行的类型名称。 |
| [SetTableRowTypeOfAll](./settablerowtypeofall/) | 设置引用表中所有行组成的表行的类型名称。 |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | 获取引用表的总计行组成的表行的类型名称。 |
| [SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | 设置引用表的总计行组成的表行的类型名称。 |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | 获取引用表中当前行组成的表行的类型名称。 |
| [SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | 设置引用表中当前行组成的表行的类型名称。 |
| [GetErrorValueString](./geterrorvaluestring/) | 获取单元格错误值的显示字符串。 |
| [GetBooleanValueString](./getbooleanvaluestring/) | 获取单元格布尔值的显示字符串。 |
| [SetBooleanValueString](./setbooleanvaluestring/) | 设置单元格布尔值的显示字符串。 |
| [GetLocalFunctionName](./getlocalfunctionname/) | 根据给定的标准函数名称获取区域设置相关的函数名称。 |
| [SetLocalFunctionName](./setlocalfunctionname/) | 设置对应于给定标准函数名称的区域设置相关函数名称。 |
| [GetStandardFunctionName](./getstandardfunctionname/) | 根据给定的区域设置相关函数名称获取标准函数名称。 |
| [SetStandardFunctionName](./setstandardfunctionname/) | 根据给定的标准函数名称设置区域设置相关的函数名称。 |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | 根据给定的标准文本获取内置名称的区域设置相关文本。 |
| [SetLocalBuiltInName](./setlocalbuiltinname/) | 使用给定的标准名称文本设置内置名称的区域设置相关文本。 |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | 根据给定的区域设置相关文本获取内置名称的标准文本。 |
| [SetStandardBuiltInName](./setstandardbuiltinname/) | 根据给定的标准函数名称设置区域设置相关的函数名称。 |
| [GetListSeparator](./getlistseparator/) | 获取列表、函数参数等的分隔符。 |
| [SetListSeparator](./setlistseparator/) | 设置列表、函数参数等的分隔符。 |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | 获取公式中数组数据行的分隔符。 |
| [SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | 设置公式中数组数据行的分隔符。 |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | 获取公式中数组行数据项的分隔符。 |
| [SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | 设置公式中数组行数据项的分隔符。 |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | 根据给定的区域设置字体样式名称，获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。 |
| [SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | 根据给定的标准函数名称设置区域设置相关的函数名称。 |
| [GetCommentTitleName](./getcommenttitlename/) | 根据评论标题类型获取区域相关的评论标题名称。 |
| [SetCommentTitleName](./setcommenttitlename/) | 根据评论标题类型获取区域相关的评论标题名称。 |
