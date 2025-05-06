---
title: Line.BeginArrowWidth
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the width of the arrowhead for the begin of a line
type: docs
url: /net/aspose.cells.drawing/line/beginarrowwidth/
---
## Line.BeginArrowWidth property

Specifies the width of the arrowhead for the begin of a line.

```csharp
public MsoArrowheadWidth BeginArrowWidth { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Begin Arrowhead Width: &amp;quot; + line.BeginArrowWidth);
public static void Property_BeginArrowWidth()
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

            // Create a line shape for the chart
            Line line = chart.Line;

            // Set arrowhead styles and widths
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Output the arrowhead styles and widths
            Console.WriteLine(&quot;Begin Arrowhead Width: &quot; + line.BeginArrowWidth);
            Console.WriteLine(&quot;End Arrowhead Width: &quot; + line.EndArrowWidth);

            // Save the workbook
            workbook.Save(&quot;MsoArrowheadWidthExample.xlsx&quot;);
        }
```

### See Also

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


