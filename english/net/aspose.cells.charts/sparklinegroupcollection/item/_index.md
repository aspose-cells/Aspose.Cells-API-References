---
title: SparklineGroupCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroupCollection property. Gets the SparklineGroup element at the specified index
type: docs
url: /net/aspose.cells.charts/sparklinegroupcollection/item/
---
## SparklineGroupCollection indexer

Gets the [`SparklineGroup`](../../sparklinegroup/) element at the specified index.

```csharp
public SparklineGroup this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Aspose.Cells.Charts.SparklineGroup group = ws.SparklineGroups[idx];
//http://www.aspose.com/community/forums/thread/255758.aspx
public void SparklineGroupCollection_Property_Item()
{
    Console.WriteLine("SparklineGroupCollection_Property_Item()");
    Workbook wb = new Workbook(FileFormatType.Xlsx); // specify the dest file type
    wb.Worksheets.Clear();

    Worksheet ws = wb.Worksheets.Add("New Sheet");
    ws.Cells["A8"].PutValue(34);
    ws.Cells["A9"].PutValue(50);
    ws.Cells["A10"].PutValue(34);

    CellArea ca = new CellArea();
    ca.StartColumn = 0;
    ca.EndColumn = 0;
    ca.StartRow = 0;
    ca.EndRow = 0;

    int idx = ws.SparklineGroups.Add(Aspose.Cells.Charts.SparklineType.Column,
     "'" + ws.Name + "'!A8:A10", true, ca);
    Aspose.Cells.Charts.SparklineGroup group = ws.SparklineGroups[idx];

    // change the color of the series if need
    CellsColor clr = wb.CreateCellsColor();
    clr.Color = Color.Orange;
    group.SeriesColor = clr;
    Util.ReSave(wb, SaveFormat.Xlsx);
    //wb.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


