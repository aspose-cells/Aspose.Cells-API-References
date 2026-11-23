---
title: "类 PivotTableFormatCollection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotTableFormatCollection 类。表示应用于数据透视表的格式集合"
type: docs
url: /zh/net/aspose.cells.pivot/pivottableformatcollection/
---
## PivotTableFormatCollection class

表示应用于数据透视表的格式集合。

```csharp
public class PivotTableFormatCollection : CollectionBase<PivotTableFormat>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivottableformatcollection/item/) { get; } | 按索引获取格式。 |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivottableformatcollection/add/)() | 添加一个[`PivotTableFormat`](../pivottableformat/)。 |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTableFormat) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTableFormat, IComparer&lt;PivotTableFormat&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotTableFormat, IComparer&lt;PivotTableFormat&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotTableFormat) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTableFormat[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTableFormat[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotTableFormat[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotTableFormat&gt;) |  |
| [Format](../../aspose.cells.pivot/pivottableformatcollection/format/#format)(CellArea, Style) | 格式化数据透视表的选定区域。 |
| [Format](../../aspose.cells.pivot/pivottableformatcollection/format/#format_1)(PivotArea, Style) | 格式化数据透视表的选定区域。 |
| [Format](../../aspose.cells.pivot/pivottableformatcollection/format/#format_2)(int, int, Style) | 格式化数据透视表区域中的单元格 |
| [FormatArea](../../aspose.cells.pivot/pivottableformatcollection/formatarea/)(PivotFieldType, int, PivotFieldSubtotalType, PivotTableSelectionType, bool, bool, Style) | 格式化选定区域。 |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableFormatCollectionDemo
    {
        public static void PivotTableFormatCollectionExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加一些数据
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // 向工作表添加透视表
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // 访问 PivotTableFormatCollection
            PivotTableFormatCollection formatCollection = pivotTable.PivotFormats;

            // 向集合添加格式
            int formatIndex = formatCollection.Add();
            PivotTableFormat pivotFormat = formatCollection[formatIndex];

            // 定义格式区域
            PivotTableFormat newFormat = formatCollection.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, new Style());

            // 设置格式的样式
            Style style = new Style();
            style.BackgroundColor = Color.LightBlue;
            newFormat.SetStyle(style);

            // 保存工作簿
            workbook.Save("PivotTableFormatCollectionExample.xlsx");
        }
    }
}
```

### 另请参见

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotTableFormat](../pivottableformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


