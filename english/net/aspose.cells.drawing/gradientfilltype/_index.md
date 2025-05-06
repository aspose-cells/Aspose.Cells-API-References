---
title: Enum GradientFillType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GradientFillType enum. Represents all Gradient fill type
type: docs
url: /net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Represents all Gradient fill type.

```csharp
public enum GradientFillType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Linear | `0` | Linear |
| Radial | `1` | Radial |
| Rectangle | `2` | Rectangle |
| Path | `3` | Path |

### Examples

```csharp
// Called: fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);
public static void Type_GradientFillType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Access the chart&apos;s plot area
            PlotArea plotArea = chart.PlotArea;

            // Access the fill format of the plot area
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Set a two-color gradient fill with a specific direction
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Output the gradient direction type
            Console.WriteLine(&quot;Gradient Direction Type: &quot; + fillFormat.GradientFill.DirectionType);

            // Save the workbook
            workbook.Save(&quot;GradientDirectionTypeExample.xlsx&quot;);
            workbook.Save(&quot;GradientDirectionTypeExample.pdf&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


