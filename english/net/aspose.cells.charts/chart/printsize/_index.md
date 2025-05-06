---
title: Chart.PrintSize
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets the printed chart size
type: docs
url: /net/aspose.cells.charts/chart/printsize/
---
## Chart.PrintSize property

Gets and sets the printed chart size.

```csharp
public PrintSizeType PrintSize { get; set; }
```

### Examples

```csharp
// Called: chart.PrintSize = PrintSizeType.Fit;
public static void Property_PrintSize()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Get the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[0, 0].PutValue(&quot;Category&quot;);
            worksheet.Cells[0, 1].PutValue(&quot;Value&quot;);
            worksheet.Cells[1, 0].PutValue(&quot;A&quot;);
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue(&quot;B&quot;);
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue(&quot;C&quot;);
            worksheet.Cells[3, 1].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the data range for the chart
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Set the chart title
            chart.Title.Text = &quot;Sample Chart&quot;;

            // Set the print size of the chart
            chart.PrintSize = PrintSizeType.Fit;

            // Save the workbook
            workbook.Save(&quot;PrintSizeTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* enum [PrintSizeType](../../../aspose.cells/printsizetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


