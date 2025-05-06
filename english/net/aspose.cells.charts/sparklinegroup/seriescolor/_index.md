---
title: SparklineGroup.SeriesColor
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the color of the sparklines in the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/seriescolor/
---
## SparklineGroup.SeriesColor property

Gets and sets the color of the sparklines in the sparkline group.

```csharp
public CellsColor SeriesColor { get; set; }
```

### Examples

```csharp
// Called: group.SeriesColor = clr;
[Test]
        //http://www.aspose.com/community/forums/thread/258337.aspx
        public void Property_SeriesColor()
        {
            Console.WriteLine(&quot;Property_SeriesColor()&quot;);
            Workbook wb = new Workbook(FileFormatType.Xlsx); // specify the dest file type
            wb.Worksheets.Clear();
            Worksheet ws = wb.Worksheets.Add(&quot;New Sheet&quot;);
            ws.Cells[&quot;A8&quot;].PutValue(34);
            ws.Cells[&quot;B8&quot;].PutValue(50);
            ws.Cells[&quot;C8&quot;].PutValue(34);
            CellArea ca = new CellArea();
            ca.StartColumn = 9;
            ca.EndColumn = 9;
            ca.StartRow = 6;
            ca.EndRow = 6;
            int idx = ws.SparklineGroups.Add(Aspose.Cells.Charts.SparklineType.Column, &quot;&apos;&quot; + ws.Name + &quot;&apos;!A8:C8&quot;, false, ca);
            Aspose.Cells.Charts.SparklineGroup group = ws.SparklineGroups[idx];
            //ws.Cells[&quot;A10&quot;].PutValue(50);
            //ws.Cells[&quot;B10&quot;].PutValue(34);
            //ws.Cells[&quot;C10&quot;].PutValue(50);
            //ca = new CellArea();
            //ca.StartColumn = 9;
            //ca.EndColumn = 9;
            //ca.StartRow = 5;
            //ca.EndRow = 5;
            //idx = ws.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Column, &quot;&apos;&quot; + ws.Name + &quot;&apos;!A10:C10&quot;, false, ca);
            //group = ws.SparklineGroupCollection[idx];
            // change the color of the series if need
            CellsColor clr = wb.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;
            ws.Cells.InsertRows(2, 17);
            //ws.Cells.DeleteRows(5, 2);
            Util.ReSave(wb, SaveFormat.Xlsx);
            //wb.Save(Constants.destPath + @&quot;CELLSNET-19722.xlsx&quot;);
        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


