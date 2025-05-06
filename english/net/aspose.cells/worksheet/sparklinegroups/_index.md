---
title: Worksheet.SparklineGroups
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the sparkline groups in the worksheet
type: docs
url: /net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Gets the sparkline groups in the worksheet.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Examples

```csharp
// Called: int idx = ws.SparklineGroups.Add(Aspose.Cells.Charts.SparklineType.Column,
[Test]
        //http://www.aspose.com/community/forums/thread/255758.aspx
        public void Property_SparklineGroups()
        {
            Console.WriteLine(&quot;Property_SparklineGroups()&quot;);
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
            //wb.Save(Constants.destPath + @&quot;CELLSNET-19619.xlsx&quot;);
        }
```

### See Also

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


