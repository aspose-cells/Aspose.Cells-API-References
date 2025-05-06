---
title: Line.DashType
second_title: Aspose.Cells for .NET API Reference
description: Line property. Specifies the dash line type
type: docs
url: /net/aspose.cells.drawing/line/dashtype/
---
## Line.DashType property

Specifies the dash line type

```csharp
public MsoLineDashStyle DashType { get; set; }
```

### Examples

```csharp
// Called: categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;
public static void Property_DashType()
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

            // Set the dash style of the major gridlines
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Set the dash style of the minor gridlines
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Save the workbook
            workbook.Save(&quot;MsoLineDashStyleExample.xlsx&quot;);

            // Output the results
            Console.WriteLine(&quot;Chart with custom dash styles for gridlines created successfully.&quot;);
        }
```

### See Also

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


