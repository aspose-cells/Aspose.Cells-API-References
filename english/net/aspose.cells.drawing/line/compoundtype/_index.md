---
title: Line.CompoundType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the compound line type
type: docs
url: /net/aspose.cells.drawing/line/compoundtype/
---
## Line.CompoundType property

Specifies the compound line type

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Examples

```csharp
// Called: axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
public static void Property_CompoundType()
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

            // Access the primary category axis
            Axis categoryAxis = chart.CategoryAxis;

            // Set the line style for the primary category axis
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Output the line style
            Console.WriteLine(&quot;Axis Line Style: &quot; + axisLine.CompoundType);
            Console.WriteLine(&quot;Axis Line Color: &quot; + axisLine.Color);
            Console.WriteLine(&quot;Axis Line Weight: &quot; + axisLine.WeightPt);

            // Save the workbook
            workbook.Save(&quot;MsoLineStyleExample.xlsx&quot;);
        }
```

### See Also

* enum [MsoLineStyle](../../msolinestyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


