---
title: Chart.Line
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the line
type: docs
url: /net/aspose.cells.charts/chart/line/
---
## Chart.Line property

Gets the line.

```csharp
public Line Line { get; }
```

### Examples

```csharp
// Called: Line line = chart.Line;
public static void Property_Line()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Create a line shape for the chart
            Line line = chart.Line;

            // Set the arrowhead lengths
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Output the arrowhead lengths
            Console.WriteLine(&quot;Begin Arrowhead Length: &quot; + line.BeginArrowLength);
            Console.WriteLine(&quot;End Arrowhead Length: &quot; + line.EndArrowLength);

            // Save the workbook
            workbook.Save(&quot;MsoArrowheadLengthExample.xlsx&quot;);
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


