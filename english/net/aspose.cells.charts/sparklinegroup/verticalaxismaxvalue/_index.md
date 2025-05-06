---
title: SparklineGroup.VerticalAxisMaxValue
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets and sets the custom maximum value for the vertical axis
type: docs
url: /net/aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/
---
## SparklineGroup.VerticalAxisMaxValue property

Gets and sets the custom maximum value for the vertical axis.

```csharp
public double VerticalAxisMaxValue { get; set; }
```

### Examples

```csharp
// Called: group.VerticalAxisMaxValue = 10.0;
public static void Property_VerticalAxisMaxValue()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells[&quot;A1&quot;].PutValue(5);
            sheet.Cells[&quot;B1&quot;].PutValue(2);
            sheet.Cells[&quot;C1&quot;].PutValue(1);
            sheet.Cells[&quot;D1&quot;].PutValue(3);

            // Define the CellArea for the sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Add a sparkline group to the worksheet
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, &quot;A1:D1&quot;, false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Add sparklines to the group
            group.Sparklines.Add(sheet.Name + &quot;!A1:D1&quot;, 0, 4);

            // Create CellsColor for series color
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Set the high points are colored green and the low points are colored red
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            group.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            group.LowPointColor = lowPointColor;

            // Set line weight
            group.LineWeight = 1.0;

            // Set additional properties
            group.PresetStyle = SparklinePresetStyleType.Style1;
            group.Type = SparklineType.Line;
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
            group.DisplayHidden = true;
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            group.ShowMarkers = true;
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            group.PlotRightToLeft = false;
            CellsColor horizontalAxisColor = workbook.CreateCellsColor();
            horizontalAxisColor.Color = Color.Gray;
            group.HorizontalAxisColor = horizontalAxisColor;

            group.ShowHorizontalAxis = true;
            group.HorizontalAxisDateRange = &quot;A1:D1&quot;;
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMinValue = 0.0;

            // Save the workbook
            workbook.Save(&quot;SparklineGroupExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


