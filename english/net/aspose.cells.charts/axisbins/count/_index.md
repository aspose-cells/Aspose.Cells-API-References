---
title: AxisBins.Count
second_title: Aspose.Cells for .NET API Reference
description: AxisBins property. Gets or set the count of axis bins
type: docs
url: /net/aspose.cells.charts/axisbins/count/
---
## AxisBins.Count property

Gets or set the count of axis bins

```csharp
public int Count { get; set; }
```

### Examples

```csharp
// Called: bins.Count = 5;
public static void Property_Count()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Add a new worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Add data series to the chart
            chart.NSeries.Add("A1:A5", true);

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
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
```

### See Also

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


