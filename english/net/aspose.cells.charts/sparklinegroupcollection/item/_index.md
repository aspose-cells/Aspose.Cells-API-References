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
public void Property_Int32_()
        {
            Console.WriteLine(&quot;Property_Int32_()&quot;);
            Workbook wb = new Workbook(FileFormatType.Xlsx); // specify the dest file type
            wb.Worksheets.Clear();
            Worksheet ws = wb.Worksheets.Add(&quot;New Sheet&quot;);
            ws.Cells[&quot;A8&quot;].PutValue(34);
            ws.Cells[&quot;A9&quot;].PutValue(50);
            ws.Cells[&quot;A10&quot;].PutValue(34);
            CellArea ca = new CellArea();
            ca.StartColumn = 0;
            ca.EndColumn = 0;
            ca.StartRow = 0;
            ca.EndRow = 0;
            int idx = ws.SparklineGroups.Add(Aspose.Cells.Charts.SparklineType.Column,
             &quot;&apos;&quot; + ws.Name + &quot;&apos;!A8:A10&quot;, true, ca);
            Aspose.Cells.Charts.SparklineGroup group = ws.SparklineGroups[idx];
            // change the color of the series if need
            CellsColor clr = wb.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;
            Util.ReSave(wb, SaveFormat.Xlsx);
            //wb.Save(Constants.destPath + &quot;Test_CreateSparkline_out.xlsx&quot;);
        }
```

### See Also

* class [SparklineGroup](../../sparklinegroup/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


