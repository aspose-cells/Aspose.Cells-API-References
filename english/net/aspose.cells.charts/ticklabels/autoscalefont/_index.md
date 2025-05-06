---
title: TickLabels.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: tickLabels.AutoScaleFont = true;
public static void Property_AutoScaleFont()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(4);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Access the value axis
            Axis valueAxis = chart.ValueAxis;

            // Access the tick labels of the value axis
            TickLabels tickLabels = valueAxis.TickLabels;

            // Set properties of the tick labels
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = &quot;0.00&quot;;
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Save the workbook
            workbook.Save(&quot;TickLabelsExample.xlsx&quot;);
        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


