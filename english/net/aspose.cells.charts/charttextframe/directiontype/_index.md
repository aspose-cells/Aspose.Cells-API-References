---
title: ChartTextFrame.DirectionType
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets and sets the direction of text
type: docs
url: /net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Gets and sets the direction of text.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Examples

```csharp
// Called: legend.DirectionType = ChartTextDirectionType.Horizontal;
public static void Property_DirectionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Get the first worksheet
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue(&quot;Income&quot;);
            cells[1, 0].PutValue(&quot;Company A&quot;);
            cells[2, 0].PutValue(&quot;Company B&quot;);
            cells[3, 0].PutValue(&quot;Company C&quot;);
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Add a chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Access the legend of the chart
            Legend legend = chart.Legend;

            // Set legend properties
            legend.Position = LegendPositionType.Left;
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;
            legend.IsOverLay = false;
            legend.IsAutoText = true;
            legend.IsDeleted = false;
            legend.TextHorizontalAlignment = TextAlignmentType.Center;
            legend.TextVerticalAlignment = TextAlignmentType.Center;
            legend.RotationAngle = 0;
            legend.Text = &quot;Legend Text&quot;;
            legend.LinkedSource = &quot;Sheet1!A1&quot;;
            legend.TextDirection = TextDirectionType.LeftToRight;
            legend.ReadingOrder = TextDirectionType.Context;
            legend.DirectionType = ChartTextDirectionType.Horizontal;
            legend.IsTextWrapped = true;
            legend.IsResizeShapeToFitText = true;
            legend.IsInnerMode = false;
            legend.AutoScaleFont = true;
            legend.BackgroundMode = BackgroundMode.Transparent;
            legend.IsAutomaticSize = true;
            legend.X = 100;
            legend.Y = 100;
            legend.Height = 200;
            legend.Width = 200;
            legend.Shadow = true;

            // Save the workbook
            workbook.Save(&quot;LegendExample.xlsx&quot;);
            workbook.Save(&quot;LegendExample.pdf&quot;);
        }
```

### See Also

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


