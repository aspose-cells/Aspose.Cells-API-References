---
title: Class PivotFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFilterCollection class. Represents a collection of all the PivotFilters
type: docs
url: /net/aspose.cells.pivot/pivotfiltercollection/
---
## PivotFilterCollection class

Represents a collection of all the PivotFilters.

```csharp
public class PivotFilterCollection : CollectionBase<PivotFilter>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivotfiltercollection/item/) { get; } | Gets the pivotfilter object at the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivotfiltercollection/add/)(int, PivotFilterType) | (**Obsolete.**) Adds a PivotFilter Object to the specific type |
| [AddDateFilter](../../aspose.cells.pivot/pivotfiltercollection/adddatefilter/)(int, PivotFilterType, DateTime, DateTime) | Filters by date setting of row or column pivot field. |
| [AddLabelFilter](../../aspose.cells.pivot/pivotfiltercollection/addlabelfilter/)(int, PivotFilterType, string, string) | Filters by captions of row or column pivot field. |
| [AddTop10Filter](../../aspose.cells.pivot/pivotfiltercollection/addtop10filter/)(int, int, PivotFilterType, bool, int) | Filters by values of data pivot field. |
| [AddValueFilter](../../aspose.cells.pivot/pivotfiltercollection/addvaluefilter/)(int, int, PivotFilterType, double, double) | Filters by values of data pivot field. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotFilter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotFilter, IComparer&lt;PivotFilter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotFilter, IComparer&lt;PivotFilter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [ClearFilter](../../aspose.cells.pivot/pivotfiltercollection/clearfilter/)(int) | Clear PivotFilter from the specific PivotField |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotFilter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotFilter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotFilter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotFilter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotFilter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotFilter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotFilter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotFilter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotFilter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotFilter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotFilter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotFilter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotFilter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotFilter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionDemo
    {
        public static void PivotFilterCollectionExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Access the PivotFilterCollection
            PivotFilterCollection pivotFilters = pivotTable.PivotFilters;

            // Add a filter to the pivot table
            int filterIndex = pivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotFilters[filterIndex];

            // Set some properties of the filter
            filter.Value1 = "50";
            filter.Value2 = "100";
            filter.MeasureFldIndex = 2; // Assuming the measure field index is 2

            // Save the workbook
            workbook.Save("PivotFilterCollectionExample.xlsx");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotFilter](../pivotfilter/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


