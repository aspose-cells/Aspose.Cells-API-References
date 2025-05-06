---
title: SparklineGroup.LowPointColor
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the color of the lowest points of data in the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/lowpointcolor/
---
## SparklineGroup.LowPointColor property

Gets and sets the color of the lowest points of data in the sparkline group.

```csharp
public CellsColor LowPointColor { get; set; }
```

### Examples

```csharp
// Called: sparklineGroup.LowPointColor = lowPointColor;
public static void Property_LowPointColor()
        {
            // Create a workbook and a worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(5);
            worksheet.Cells[&quot;B1&quot;].PutValue(2);
            worksheet.Cells[&quot;C1&quot;].PutValue(1);
            worksheet.Cells[&quot;D1&quot;].PutValue(3);

            // Define the CellArea
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, &quot;A1:D1&quot;, false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
            sparklineGroup.Sparklines.Add(worksheet.Name + &quot;!A1:D1&quot;, 0, 4);

            // Set properties for the sparkline group
            sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Create CellsColor
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Set additional properties
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;
            sparklineGroup.LineWeight = 1.0;

            // Save the workbook
            workbook.Save(&quot;SparklineAxisMinMaxTypeExample.xlsx&quot;);
        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


