---
title: Class PivotFormatConditionCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFormatConditionCollection class. Represents PivotTable Format Conditions
type: docs
url: /net/aspose.cells.pivot/pivotformatconditioncollection/
---
## PivotFormatConditionCollection class

Represents PivotTable Format Conditions.

```csharp
public class PivotFormatConditionCollection : CollectionBase<PivotFormatCondition>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotformatconditioncollection/item/) { get; } | Gets the pivot FormatCondition object at the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotformatconditioncollection/add/)() | Adds a pivot FormatCondition to the collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotFormatCondition) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotFormatCondition, IComparer&lt;PivotFormatCondition&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotFormatCondition, IComparer&lt;PivotFormatCondition&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotFormatCondition) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotFormatCondition[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotFormatCondition[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotFormatCondition[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotFormatCondition&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotFormatCondition&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotFormatCondition&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotFormatCondition) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotFormatCondition, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotFormatCondition, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotFormatCondition) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotFormatCondition, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotFormatCondition, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotFormatConditionCollectionDemo
    {
        public static void PivotFormatConditionCollectionExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[4, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C5", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Configure the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Add a pivot format condition
            PivotFormatConditionCollection pivotFormatConditions = pivotTable.PivotFormatConditions;
            int formatConditionIndex = pivotFormatConditions.Add();
            PivotFormatCondition pivotFormatCondition = pivotFormatConditions[formatConditionIndex];

            // Configure the format condition
            FormatConditionCollection formatConditions = pivotFormatCondition.FormatConditions;
            formatConditions.AddArea(pivotTable.DataBodyRange);
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            formatCondition.Formula1 = "60";
            formatCondition.Operator = OperatorType.GreaterOrEqual;
            formatCondition.Style.BackgroundColor = Color.Yellow;

            // Save the workbook
            workbook.Save("PivotFormatConditionCollectionExample.xlsx");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotFormatCondition](../pivotformatcondition/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


