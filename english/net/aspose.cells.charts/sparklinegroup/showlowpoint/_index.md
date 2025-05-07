---
title: SparklineGroup.ShowLowPoint
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Indicates whether to highlight the lowest points of data in the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/showlowpoint/
---
## SparklineGroup.ShowLowPoint property

Indicates whether to highlight the lowest points of data in the sparkline group.

```csharp
public bool ShowLowPoint { get; set; }
```

### Examples

```csharp
// Called: sparklineGroup.ShowLowPoint = true;
public static void Property_ShowLowPoint()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Insert sample data into the worksheet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Define the CellArea where the sparklines will be added
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Add a new SparklineGroup to the worksheet
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            // Add sparklines to the SparklineGroup
            sparklineGroup.Sparklines.Add("A1:D1", 0, 4);

            // Set various properties for the SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Set colors for high and low points
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Set the series color and line weight
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;

            // Save the workbook
            workbook.Save("SparklineCollectionExample.xlsx");
        }
```

### See Also

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


