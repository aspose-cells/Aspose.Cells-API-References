---
title: GlobalizationSettings
second_title: Aspose.Cells for .NET API 参考
description: 代表全球化设置
type: docs
weight: 3620
url: /zh/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

代表全球化设置。

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | 获取或设置此图表[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | 获取公式中数组行数据中项目的分隔符。 |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | 获取列表、函数参数等的分隔符。 |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | 获取公式中数组数据中行的分隔符。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | 根据一定的排序规则比较两个字符串值。 |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | 获取数据透视表中“（全部）”标签的名称。 |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | 获取单元格布尔值的显示字符串值 |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | 根据某些排序规则将字符串转换为可比较的对象。 |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | 获取数据透视表中“列标签”标签的名称。 |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | 根据评论标题类型获取依赖语言环境的评论标题名称。 |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | 获取数据透视表中“（空白）”标签的名称。 |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | 获取单元格错误值的显示字符串值 |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | 获取函数的总名称。 |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | 根据给定的标准文本获取内置名称的区域设置相关文本。 |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | 根据给定的标准函数名获取与语言环境相关的函数名。 |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | 获取数据透视表中“（多个项目）”标签的名称。 |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | 获取饼图的“其他”标签的名称。 |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | 获取数据透视表中“总计”标签的名称。 |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | 获取数据透视表中“总计”标签的名称。 当数据透视表的数据区域包含两个或多个数据透视字段时，需要重写此方法。 |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | 获取数据透视表中的保护名称。 |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | 获取数据透视表中“行标签”标签的名称。 |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | 根据给定的区域设置相关文本获取内置名称的标准文本。 |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | 根据给定的区域设置相关函数名称获取标准函数名称。 |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | 根据给定的区域设置字体样式名称获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。 |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | 获取名称[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype)输入数据透视表. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | 获取由引用表中所有行组成的表行的类型名称。 默认为“All”，因此公式中“#All”表示引用表中的所有行。 |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | 获取引用表中包含当前行的表行的类型名称。 默认为“This Row”，因此公式中“#This Row”表示引用表中的当前行。 |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | 获取由引用表的数据区域组成的表行的类型名称。 默认为“数据”，因此公式中“#Data”表示表的数据区域。 |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | 获取由表头组成的表行的类型名称。 默认为“Headers”，因此公式中“#Headers”代表表头。 |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | 获取由引用表的总行组成的表行的类型名称。 默认为“Totals”，因此公式中“#Totals”表示引用表的总行。 |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | 获取函数的总名称。 |

### 也可以看看

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
