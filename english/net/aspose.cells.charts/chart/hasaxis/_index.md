---
title: Chart.HasAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Returns which axes exist on the chart
type: docs
url: /net/aspose.cells.charts/chart/hasaxis/
---
## Chart.HasAxis method

Returns which axes exist on the chart.

```csharp
public bool HasAxis(AxisType aixsType, bool isPrimary)
```

### Remarks

Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded is no axis.

### Examples

```csharp
// Called: bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
public static void Method_Boolean_()
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

            // Determine which axes exist in the chart
            bool hasPrimaryCategoryAxis = chart.HasAxis(AxisType.Category, true);
            bool hasSecondaryCategoryAxis = chart.HasAxis(AxisType.Category, false);
            bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
            bool hasSecondaryValueAxis = chart.HasAxis(AxisType.Value, false);

            // Output the results
            Console.WriteLine(&quot;Has Primary Category Axis: &quot; + hasPrimaryCategoryAxis);
            Console.WriteLine(&quot;Has Secondary Category Axis: &quot; + hasSecondaryCategoryAxis);
            Console.WriteLine(&quot;Has Primary Value Axis: &quot; + hasPrimaryValueAxis);
            Console.WriteLine(&quot;Has Secondary Value Axis: &quot; + hasSecondaryValueAxis);

            // Save the workbook
            workbook.Save(&quot;AxisTypeExample.xlsx&quot;);
            workbook.Save(&quot;AxisTypeExample.pdf&quot;);
        }
```

### See Also

* enum [AxisType](../../axistype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


