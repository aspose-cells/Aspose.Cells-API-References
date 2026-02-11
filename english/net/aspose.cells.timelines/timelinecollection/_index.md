---
title: Class TimelineCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Timelines.TimelineCollection class. Specifies the collection of all the Timeline objects on the worksheet. It was supported since Excel 2013
type: docs
url: /net/aspose.cells.timelines/timelinecollection/
---
## TimelineCollection class

Specifies the collection of all the [`Timeline`](../timeline/) objects on the worksheet. It was supported since Excel 2013.

```csharp
public class TimelineCollection : CollectionBase<Timeline>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.timelines/timelinecollection/item/) { get; } | Gets the Timeline by index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.timelines/timelinecollection/add/#add_4)(PivotTable, string, int) | Add a new Timeline using PivotTable as data source |
| [Add](../../aspose.cells.timelines/timelinecollection/add/#add_3)(PivotTable, string, PivotField) | Add a new Timeline using PivotTable as data source |
| [Add](../../aspose.cells.timelines/timelinecollection/add/#add_5)(PivotTable, string, string) | Add a new Timeline using PivotTable as data source |
| [Add](../../aspose.cells.timelines/timelinecollection/add/#add_1)(PivotTable, int, int, int) | Add a new Timeline using PivotTable as data source |
| [Add](../../aspose.cells.timelines/timelinecollection/add/#add)(PivotTable, int, int, PivotField) | Add a new Timeline using PivotTable as data source |
| [Add](../../aspose.cells.timelines/timelinecollection/add/#add_2)(PivotTable, int, int, string) | Add a new Timeline using PivotTable as data source |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Timeline) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Timeline, IComparer&lt;Timeline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Timeline, IComparer&lt;Timeline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Timeline) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Timeline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Timeline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Timeline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Timeline&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Timeline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Timeline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Timeline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Timeline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Timeline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Timeline) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Timeline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Timeline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Timeline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Timeline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Timeline, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineCollectionDemo
    {
        public static void TimelineCollectionExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Create date style
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);

            // Set date style
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Add a PivotTable
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Refresh PivotTable data
            pivot.RefreshData();
            pivot.CalculateData();

            // Add a Timeline to the worksheet
            TimelineCollection timelines = sheet.Timelines;
            int timelineIndex = timelines.Add(pivot, "A20", "date");

            // Access the added Timeline
            Timeline timeline = timelines[timelineIndex];

            // Save the workbook
            workbook.Save("TimelineCollectionExample.xlsx");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Timeline](../timeline/)
* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


