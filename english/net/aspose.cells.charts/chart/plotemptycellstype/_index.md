---
title: Chart.PlotEmptyCellsType
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets how to plot the empty cells
type: docs
url: /net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Gets and sets how to plot the empty cells.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Examples

```csharp
// Called: chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;
public static void Property_PlotEmptyCellsType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);
            worksheet.Cells[&quot;B4&quot;].PutValue(null); // Empty cell
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;D&quot;);
            worksheet.Cells[&quot;B5&quot;].PutValue(40);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.SetChartDataRange(&quot;A1:B5&quot;, true);

            // Set the title of the chart
            chart.Title.Text = &quot;Plot Empty Cells Example&quot;;

            // Set how to plot empty cells
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Save the workbook
            workbook.Save(&quot;PlotEmptyCellsTypeExample.xlsx&quot;);

            Console.WriteLine(&quot;Workbook saved successfully.&quot;);
        }
```

### See Also

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


