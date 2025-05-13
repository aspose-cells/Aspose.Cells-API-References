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
public static void Series_Property_UpBars()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);

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
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
```

### See Also

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


