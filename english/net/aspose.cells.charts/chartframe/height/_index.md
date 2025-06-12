---
title: ChartFrame.Height
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the height of frame in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Gets or sets the height of frame in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data source
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Access data labels
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Set Height property
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Display the height value
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Save the workbook
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


