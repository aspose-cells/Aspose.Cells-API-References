---
title: Chart.ChartDataTable
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Represents the chart data table
type: docs
url: /net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

Represents the chart data table.

```csharp
public ChartDataTable ChartDataTable { get; }
```

### Examples

```csharp
// Called: ChartDataTable chartTable = chart.ChartDataTable;
public static void Property_ChartDataTable()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding sample values to cells
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];

            // Adding NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Displaying the data table
            chart.ShowDataTable = true;

            // Getting Chart Data Table
            ChartDataTable chartTable = chart.ChartDataTable;

            // Setting Chart Data Table properties
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Saving the Excel file
            workbook.Save(&quot;ChartDataTableExample.xlsx&quot;);
            workbook.Save(&quot;ChartDataTableExample.pdf&quot;);
        }
```

### See Also

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


