---
title: "类 PivotConditionalFormatCollection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotConditionalFormatCollection 类。表示透视表的所有条件格式"
type: docs
url: /zh/net/aspose.cells.pivot/pivotconditionalformatcollection/
---
## PivotConditionalFormatCollection class

表示透视表的所有条件格式。

```csharp
public class PivotConditionalFormatCollection : CollectionBase<PivotConditionalFormat>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotconditionalformatcollection/item/) { get; } | 获取特定索引处的透视 FormatCondition 对象。 |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotconditionalformatcollection/add/#add_1)() | 向集合中添加透视 FormatCondition。 |
| [Add](../../aspose.cells.pivot/pivotconditionalformatcollection/add/#add)(int, int, PivotConditionFormatScopeType) | 将条件格式应用于必须位于数据区域的范围。 |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotConditionalFormat) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotConditionalFormat, IComparer&lt;PivotConditionalFormat&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotConditionalFormat, IComparer&lt;PivotConditionalFormat&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotConditionalFormat) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotConditionalFormat[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotConditionalFormat[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotConditionalFormat[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotConditionalFormat&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotConditionalFormat, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotConditionalFormat, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotConditionalFormatCollectionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "A";
            cells["B2"].Value = "East";
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "B";
            cells["B3"].Value = "West";
            cells["C3"].Value = 200;
            
            cells["A4"].Value = "C";
            cells["B4"].Value = "East";
            cells["C4"].Value = 300;
            
            cells["A5"].Value = "D";
            cells["B5"].Value = "West";
            cells["C5"].Value = 400;

            // 创建数据透视表
            int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // 向透视区域添加字段
            pivot.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivot.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivot.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // 刷新并计算数据透视表
            pivot.RefreshData();
            pivot.CalculateData();

            // 访问条件格式集合
            PivotConditionalFormatCollection pfcc = pivot.ConditionalFormats;
            int formatIndex = pfcc.Add();
            PivotConditionalFormat pfc = pfcc[formatIndex];
            
            // 获取透视表数据范围
            CellArea dataBodyRange = pivot.DataBodyRange;
            pfc.FormatConditions.AddArea(dataBodyRange);

            // 添加条件格式
            FormatConditionCollection fcc = pfc.FormatConditions;
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[conditionIndex];
            fc.Operator = OperatorType.Between;
            fc.Formula1 = "200";
            fc.Formula2 = "400";
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // 保存工作簿
            workbook.Save("PivotConditionalFormatDemo_out.xlsx");
        }
    }
}
```

### 另请参见

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotConditionalFormat](../pivotconditionalformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


