---
title: GradientFill.DirectionType
second_title: Aspose.Cells for .NET API Reference
description: GradientFill property. Gets the gradient direction type
type: docs
url: /net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Gets the gradient direction type.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Gradient Direction Type: &amp;quot; + fillFormat.GradientFill.DirectionType);
public static void Property_DirectionType()
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

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


