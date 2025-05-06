---
title: AxisBins.IsAutomatic
second_title: Aspose.Cells for .NET API Reference
description: AxisBins property. Indicates whether the axis bins are automatic
type: docs
url: /net/aspose.cells.charts/axisbins/isautomatic/
---
## AxisBins.IsAutomatic property

Indicates whether the axis bins are automatic.

```csharp
public bool IsAutomatic { get; set; }
```

### Examples

```csharp
// Called: bins.IsAutomatic = true;
public static void Property_IsAutomatic()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Add a new worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(10);
            worksheet.Cells[&quot;A2&quot;].PutValue(20);
            worksheet.Cells[&quot;A3&quot;].PutValue(30);
            worksheet.Cells[&quot;A4&quot;].PutValue(40);
            worksheet.Cells[&quot;A5&quot;].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Add data series to the chart
            chart.NSeries.Add(&quot;A1:A5&quot;, true);

            // Access the value axis
            Axis valueAxis = chart.ValueAxis;

            // Access the bins of the value axis
            AxisBins bins = valueAxis.Bins;

            // Set properties for the bins
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Reset overflow and underflow
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Save the workbook
            workbook.Save(&quot;AxisBinsExample.xlsx&quot;);
            workbook.Save(&quot;AxisBinsExample.pdf&quot;);
        }
```

### See Also

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


