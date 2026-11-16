---
title: "GlobalizationSettings 类"
linktitle: "GlobalizationSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GlobalizationSettings 类。封装了在 Go 中表示 globalizationsettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

表示全局化设置。

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetChartSettings](./getchartsettings/) | 获取图表的全局化设置。 |
| [SetChartSettings](./setchartsettings/) | 设置图表的全局化设置。 |
| [GetPivotSettings](./getpivotsettings/) | 获取数据透视表的全局化设置。 |
| [SetPivotSettings](./setpivotsettings/) | 设置数据透视表的全局化设置。 |
| [GetTotalName](./gettotalname/) | 获取函数的总名称。 |
| [GetGrandTotalName](./getgrandtotalname/) | 获取函数的总计名称。 |
| [GetDefaultSheetName](./getdefaultsheetname/) | 获取自动添加工作表时的默认工作表名称。默认值为 "Sheet"。 |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | 获取由表头组成的表行的类型名称。默认是 "Headers"，因此在公式中 "#Headers" 代表表头。 |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | 获取由引用表的数据区域组成的表行的类型名称。默认是 "Data"，因此在公式中 "#Data" 代表表的数据区域。 |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | 获取引用表中所有行的表行类型名称。默认值为 "All"，因此在公式 "#All" 中表示引用表的所有行。 |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | 获取引用表中总行的表行类型名称。默认值为 "Totals"，因此在公式 "#Totals" 中表示引用表的总行。 |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | 获取引用表中当前行的表行类型名称。默认值为 "This Row"，因此在公式 "#This Row" 中表示引用表的当前行。 |
| [GetErrorValueString](./geterrorvaluestring/) | 获取单元格错误值的显示字符串。 |
| [GetBooleanValueString](./getbooleanvaluestring/) | 获取单元格布尔值的显示字符串。 |
| [GetLocalFunctionName](./getlocalfunctionname/) | 根据给定的标准函数名称获取区域设置相关的函数名称。 |
| [GetStandardFunctionName](./getstandardfunctionname/) | 根据给定的区域设置相关函数名称获取标准函数名称。 |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | 根据给定的标准文本获取内置名称的区域设置相关文本。 |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | 根据给定的区域设置相关文本获取内置名称的标准文本。 |
| [GetListSeparator](./getlistseparator/) | 获取列表、函数参数等的分隔符。 |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | 获取公式中数组数据行的分隔符。 |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | 获取公式中数组行数据项的分隔符。 |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | 根据给定的区域设置字体样式名称，获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。 |
| [GetCommentTitleName](./getcommenttitlename/) | 根据评论标题类型获取区域相关的评论标题名称。 |
| [Compare](./compare/) | 根据特定的排序规则比较两个字符串值。 |
