---
title: SparklineGroup.HighPointColor
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the color of the highest points of data in the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/highpointcolor/
---
## SparklineGroup.HighPointColor property

Gets and sets the color of the highest points of data in the sparkline group.

```csharp
public CellsColor HighPointColor { get; set; }
```

### Examples

```csharp
// Called: group.HighPointColor.Color = Color.Green;
public static void Property_HighPointColor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(5);
            worksheet.Cells[&quot;B1&quot;].PutValue(2);
            worksheet.Cells[&quot;C1&quot;].PutValue(1);
            worksheet.Cells[&quot;D1&quot;].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, &quot;A1:D1&quot;, false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Add sparklines to the group
            group.Sparklines.Add(worksheet.Name + &quot;!A1:D1&quot;, 0, 4);

            // Customize the sparkline group
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Set the high points to be colored green and the low points to be colored red
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Set line weight
            group.LineWeight = 1.0;

            // Save the workbook
            workbook.Save(&quot;SparklineTypeExample.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


