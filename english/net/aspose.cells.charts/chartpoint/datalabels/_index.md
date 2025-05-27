---
title: ChartPoint.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Returns a DataLabels object that represents the data label associated with this chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Returns a `DataLabels` object that represents the data label associated with this chart point.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for the chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Add a column chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Set data range for the chart
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Enable data labels
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Change font color for all data labels
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;

            // Apply the font settings to all data labels
            series.DataLabels.ApplyFont();

            // Save the workbook
            workbook.Save("ChartDataLabelsDemo.xlsx");
        }
    }
}
```

### See Also

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


