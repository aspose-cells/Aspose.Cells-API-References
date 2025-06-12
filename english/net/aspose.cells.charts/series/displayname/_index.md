---
title: Series.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the seriess name that displays on the chart graph
type: docs
url: /net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Gets the series's name that displays on the chart graph.

```csharp
public string DisplayName { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("Cat3");
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Set chart data range
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Set display name for the first series by setting the Name property
            chart.NSeries[0].Name = "Sample Series Display Name";
            
            // Output the display name
            Console.WriteLine("Series Display Name: " + chart.NSeries[0].Name);
            
            // Save the workbook
            workbook.Save("SeriesDisplayNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


