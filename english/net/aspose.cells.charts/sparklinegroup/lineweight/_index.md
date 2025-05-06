---
title: SparklineGroup.LineWeight
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the line weight in each line sparkline in the sparkline group in the unit of points
type: docs
url: /net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```csharp
public double LineWeight { get; set; }
```

### Examples

```csharp
// Called: sparklineGroup.LineWeight = 1.0;
public static void Property_LineWeight()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Insert sample data into the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(5);
            worksheet.Cells[&quot;B1&quot;].PutValue(2);
            worksheet.Cells[&quot;C1&quot;].PutValue(1);
            worksheet.Cells[&quot;D1&quot;].PutValue(3);

            // Define the CellArea where the sparklines will be added
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Add a new SparklineGroup to the worksheet
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, &quot;A1:D1&quot;, false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            // Add sparklines to the SparklineGroup
            sparklineGroup.Sparklines.Add(&quot;A1:D1&quot;, 0, 4);

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
            workbook.Save(&quot;SparklineCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


