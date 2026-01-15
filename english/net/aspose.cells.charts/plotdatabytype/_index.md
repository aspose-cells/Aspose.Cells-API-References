---
title: Enum PlotDataByType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.PlotDataByType enum. Represents the type of data plot by row or column
type: docs
url: /net/aspose.cells.charts/plotdatabytype/
---
## PlotDataByType enumeration

Represents the type of data plot by row or column.

```csharp
public enum PlotDataByType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Row | `0` | By row. |
| Column | `1` | By column. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassPlotDataByTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data to the worksheet
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value1");
                worksheet.Cells["C1"].PutValue("Value2");
                worksheet.Cells["A2"].PutValue("Row1");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["C2"].PutValue(20);
                worksheet.Cells["A3"].PutValue("Row2");
                worksheet.Cells["B3"].PutValue(30);
                worksheet.Cells["C3"].PutValue(40);

                // Add a chart to the worksheet
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Set the chart data range
                chart.NSeries.Add("B2:C3", true);

                // Demonstrate using PlotDataByType enum values
                PlotDataByType plotType = PlotDataByType.Row;
                Console.WriteLine($"Chart is currently plotting data by: {plotType}");

                // Change to plot by column
                plotType = PlotDataByType.Column;
                Console.WriteLine($"Chart is now plotting data by: {plotType}");

                // Save the workbook
                workbook.Save("PlotDataByTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with PlotDataByType demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PlotDataByType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


