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
        //http://www.aspose.com/community/forums/thread/255758.aspx
        public void Property_SeriesColor()
        {
            Console.WriteLine("Property_SeriesColor()");
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
            //wb.Save(Constants.destPath + @"CELLSNET-19619.xlsx");
        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


