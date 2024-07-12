---
title: Class SlicerCache
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slicers.SlicerCache class. Represent summary description of slicer cache
type: docs
url: /net/aspose.cells.slicers/slicercache/
---
## SlicerCache class

Represent summary description of slicer cache

```csharp
public class SlicerCache
```

## Properties

| Name | Description |
| --- | --- |
| [CrossFilterType](../../aspose.cells.slicers/slicercache/crossfiltertype/) { get; set; } | Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write |
| [List](../../aspose.cells.slicers/slicercache/list/) { get; } | Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only |
| [Name](../../aspose.cells.slicers/slicercache/name/) { get; } | Returns the name of the slicer cache. |
| [SlicerCacheItems](../../aspose.cells.slicers/slicercache/slicercacheitems/) { get; } | Returns a SlicerCacheItem collection that contains the collection of all items in the slicer cache. Read-only |
| [SourceName](../../aspose.cells.slicers/slicercache/sourcename/) { get; } | Returns the name of this slicer cache. |

### Examples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

//Get SlicerCache object of current slicer
SlicerCache slicerCache = slicer.SlicerCache;

//do your business

book.Save("out.xlsx");
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


