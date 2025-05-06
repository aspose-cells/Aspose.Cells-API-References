---
title: Line.JoinType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the joining caps
type: docs
url: /net/aspose.cells.drawing/line/jointype/
---
## Line.JoinType property

Specifies the joining caps.

```csharp
public LineJoinType JoinType { get; set; }
```

### Examples

```csharp
// Called: majorGridLines.JoinType = LineJoinType.Round;
public static void Property_JoinType()
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

            // Access the primary value axis
            Axis valueAxis = chart.ValueAxis;

            // Access the line format of the major gridlines
            Line majorGridLines = valueAxis.MajorGridLines;

            // Set the join type of the line
            majorGridLines.JoinType = LineJoinType.Round;

            // Output the join type
            Console.WriteLine(&quot;Line Join Type: &quot; + majorGridLines.JoinType);

            // Save the workbook
            workbook.Save(&quot;LineJoinTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [LineJoinType](../../linejointype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


