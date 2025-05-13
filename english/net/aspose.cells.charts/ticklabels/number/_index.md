---
title: TickLabels.Number
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Represents the format number for the TickLabels object
type: docs
url: /net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Represents the format number for the TickLabels object.

```csharp
public int Number { get; set; }
```

### Examples

```csharp
// Called: tickLabels.Number = 2;
public static void TickLabels_Property_Number()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);

            // Access the value axis
            Axis valueAxis = chart.ValueAxis;

            // Access the tick labels of the value axis
            TickLabels tickLabels = valueAxis.TickLabels;

            // Set properties of the tick labels
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Save the workbook
            workbook.Save("TickLabelsExample.xlsx");
        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


