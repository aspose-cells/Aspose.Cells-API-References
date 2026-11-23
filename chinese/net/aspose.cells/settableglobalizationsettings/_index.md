---
title: "类 SettableGlobalizationSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.SettableGlobalizationSettings 类。实现了支持用户设置/更改预定义文本的 GlobalizationSettings"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/
---
## SettableGlobalizationSettings class

实现了支持用户设置/更改预定义文本的 GlobalizationSettings。

```csharp
public class SettableGlobalizationSettings : GlobalizationSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [SettableGlobalizationSettings](settableglobalizationsettings/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings/) { get; set; } | 获取或设置图表的全球化设置。（继承自 [`GlobalizationSettings`](../globalizationsettings/)。） |
| override [ColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/) { get; } | 获取公式中数组行数据项的分隔符。 |
| override [ListSeparator](../../aspose.cells/settableglobalizationsettings/listseparator/) { get; } | 获取列表、函数参数等的分隔符。 |
| [PivotSettings](../../aspose.cells/globalizationsettings/pivotsettings/) { get; set; } | 获取或设置数据透视表的全局化设置。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| override [RowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/) { get; } | 获取公式中数组数据行的分隔符。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [Compare](../../aspose.cells/globalizationsettings/compare/)(string, string, bool) | 根据特定的排序规则比较两个字符串值。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname/)() | (**Obsolete.**) 获取数据透视表中“(All)”标签的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| override [GetBooleanValueString](../../aspose.cells/settableglobalizationsettings/getbooleanvaluestring/)(bool) | 获取单元格布尔值的显示字符串。 |
| virtual [GetCollationKey](../../aspose.cells/globalizationsettings/getcollationkey/)(string, bool) | 根据特定的排序规则将字符串转换为可比较的对象。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/)() | (**Obsolete.**) 获取数据透视表中“Column Labels”标签的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| override [GetCommentTitleName](../../aspose.cells/settableglobalizationsettings/getcommenttitlename/)(CommentTitleType) | 根据评论标题类型获取区域设置相关的评论标题名称。 |
| virtual [GetDataFieldHeaderNameOfPivotTable](../../aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/)() | (**Obsolete.**) 获取数据透视表中值区域字段标题的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetDefaultSheetName](../../aspose.cells/globalizationsettings/getdefaultsheetname/)() | 获取自动添加工作表时的默认工作表名称。默认是“Sheet”。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname/)() | (**Obsolete.**) 获取数据透视表中“(blank)”标签的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| override [GetErrorValueString](../../aspose.cells/settableglobalizationsettings/geterrorvaluestring/)(string) | 获取单元格错误值的显示字符串。 |
| override [GetGrandTotalName](../../aspose.cells/settableglobalizationsettings/getgrandtotalname/)(ConsolidationFunction) | 获取函数的总计名称。 |
| override [GetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/getlocalbuiltinname/)(string) | 根据给定的标准文本获取内置名称的区域设置相关文本。 |
| override [GetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/getlocalfunctionname/)(string) | 根据给定的标准函数名称获取区域设置相关的函数名称。 |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname/)() | (**Obsolete.**) 获取数据透视表中“(Multiple Items)”标签的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname/)() | (**Obsolete.**) 获取数据透视表中“Grand Total”标签的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname/)() | (**Obsolete.**) 获取数据透视表中“Total”标签的名称。当数据区域包含两个或更多 PivotField 时，需要重写此方法。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable/)() | (**Obsolete.**) 获取数据透视表中的保护名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/)() | (**Obsolete.**) 获取数据透视表中“Row Labels”标签的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| override [GetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/getstandardbuiltinname/)(string) | 根据给定的区域设置相关文本获取内置名称的标准文本。 |
| override [GetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/getstandardfunctionname/)(string) | 根据给定的区域设置相关函数名称获取标准函数名称。 |
| override [GetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/)(string) | 根据给定的区域设置字体样式名称获取页眉/页脚的标准英文字体样式名称（Regular、Bold、Italic）。 |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname/)(PivotFieldSubtotalType) | (**Obsolete.**) 获取数据透视表中[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) 类型的名称。（继承自[`GlobalizationSettings`](../globalizationsettings/)。） |
| override [GetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofall/)() | 获取由引用表中的所有行组成的表行的类型名称。 |
| override [GetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/)() | 获取由引用表中的当前行组成的表行的类型名称。 |
| override [GetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/)() | 获取由引用表的数据区域组成的表行的类型名称。默认是 "Data"，因此在公式中 "#Data" 代表表格的数据区域。 |
| override [GetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/gettablerowtypeofheaders/)() | 获取由表头组成的表行的类型名称。默认是 "Headers"，因此在公式中 "#Headers" 代表表头。 |
| override [GetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/gettablerowtypeoftotals/)() | 获取由引用表的合计行组成的表行的类型名称。 |
| override [GetTotalName](../../aspose.cells/settableglobalizationsettings/gettotalname/)(ConsolidationFunction) | 获取特定函数的总计名称。 |
| [SetBooleanValueString](../../aspose.cells/settableglobalizationsettings/setbooleanvaluestring/)(bool, string) | 设置单元格布尔值的显示字符串值 |
| [SetColumnSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/)(char) | 设置公式中数组行数据项的分隔符。 |
| [SetCommentTitleName](../../aspose.cells/settableglobalizationsettings/setcommenttitlename/)(CommentTitleType, string) | 根据评论标题类型获取区域设置相关的评论标题名称。 |
| [SetGrandTotalName](../../aspose.cells/settableglobalizationsettings/setgrandtotalname/)(ConsolidationFunction, string) | 设置特定函数的总计名称。 |
| [SetListSeparator](../../aspose.cells/settableglobalizationsettings/setlistseparator/)(char) | 设置列表、函数参数等的分隔符。 |
| [SetLocalBuiltInName](../../aspose.cells/settableglobalizationsettings/setlocalbuiltinname/)(string, string, bool) | 为给定的标准名称文本设置内置名称的区域性相关文本。 |
| [SetLocalFunctionName](../../aspose.cells/settableglobalizationsettings/setlocalfunctionname/)(string, string, bool) | 为给定的标准函数名称设置对应的区域性相关函数名称。 |
| [SetRowSeparatorOfFormulaArray](../../aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/)(char) | 设置公式中数组数据行的分隔符。 |
| [SetStandardBuiltInName](../../aspose.cells/settableglobalizationsettings/setstandardbuiltinname/)(string, string, bool) | 根据给定的标准函数名称设置区域性相关函数名称。 |
| [SetStandardFunctionName](../../aspose.cells/settableglobalizationsettings/setstandardfunctionname/)(string, string, bool) | 根据给定的标准函数名称设置区域性相关函数名称。 |
| [SetStandardHeaderFooterFontStyleName](../../aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/)(string, string) | 根据给定的标准函数名称设置区域性相关函数名称。 |
| [SetTableRowTypeOfAll](../../aspose.cells/settableglobalizationsettings/settablerowtypeofall/)(string) | 设置由引用表中的所有行组成的表行的类型名称。 |
| [SetTableRowTypeOfCurrent](../../aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/)(string) | 设置由引用表中的当前行组成的表行的类型名称。 |
| [SetTableRowTypeOfData](../../aspose.cells/settableglobalizationsettings/settablerowtypeofdata/)(string) | 设置由引用表的数据区域组成的表行的类型名称。 |
| [SetTableRowTypeOfHeaders](../../aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/)(string) | 设置由表头组成的表行的类型名称。 |
| [SetTableRowTypeOfTotals](../../aspose.cells/settableglobalizationsettings/settablerowtypeoftotals/)(string) | 设置由引用表的合计行组成的表行的类型名称。 |
| [SetTotalName](../../aspose.cells/settableglobalizationsettings/settotalname/)(ConsolidationFunction, string) | 设置特定函数的总计名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class CellsClassSettableGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // 设置自定义列表分隔符
            settings.SetListSeparator(';');

            // 设置自定义布尔值字符串
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // 设置自定义函数名称
            settings.SetLocalFunctionName("SUM", "SUMME", true);
            settings.SetLocalFunctionName("AVERAGE", "MITTELWERT", true);

            // 设置自定义表行类型名称
            settings.SetTableRowTypeOfHeaders("HEADERS_CUSTOM");
            settings.SetTableRowTypeOfData("DATA_CUSTOM");
            settings.SetTableRowTypeOfTotals("TOTALS_CUSTOM");

            // 设置自定义评论标题名称
            settings.SetCommentTitleName(CommentTitleType.Comment, "COMMENT_CUSTOM");
            // 已删除 作者 行，因为 CommentTitleType 没有该枚举值
            // 如果需要设置作者相关的设置，则需要改用 ThreadedCommentAuthor

            // 将全局化设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            // 演示在公式中的用法
            worksheet.Cells["A1"].Formula = "=TRUE()";
            worksheet.Cells["A2"].Formula = "=FALSE()";
            worksheet.Cells["A3"].Formula = "=SUM(1,2,3)";
            worksheet.Cells["A4"].Formula = "=AVERAGE(1,2,3)";

            // 保存工作簿
            workbook.Save("SettableGlobalizationSettingsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [GlobalizationSettings](../globalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


