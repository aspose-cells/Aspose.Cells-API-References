---
title: Series.UpBars
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts
type: docs
url: /net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.

```csharp
public DropBars UpBars { get; }
```

### Examples

```csharp
// Called: DropBars upBars = chart.NSeries[0].UpBars;
public static void Property_UpBars()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(60);
            worksheet.Cells[&quot;B2&quot;].PutValue(32);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);

            // Enable up and down bars
            chart.NSeries[0].HasUpDownBars = true;

            // Access the DropBars object
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Customize the appearance of the up bars
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Customize the appearance of the down bars
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Save the workbook
            workbook.Save(&quot;DropBarsExample.xlsx&quot;);
            workbook.Save(&quot;DropBarsExample.pdf&quot;);
        }
```

### See Also

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


