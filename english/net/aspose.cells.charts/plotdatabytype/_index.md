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

    public class PlotDataByTypeDemo
    {
        public static void PlotDataByTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.SetChartDataRange("A1:B4", true);

            // Save the workbook
            workbook.Save("PlotDataByTypeExample.xlsx");

            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


