---
title: Chart.Placement
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Represents the way the chart is attached to the cells below it
type: docs
url: /net/aspose.cells.charts/chart/placement/
---
## Chart.Placement property

Represents the way the chart is attached to the cells below it.

```csharp
public PlacementType Placement { get; set; }
```

### Examples

```csharp
// Called: chart.Placement = PlacementType.MoveAndSize;
public static void Property_Placement()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;A&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;B&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;C&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange(&quot;A1:B4&quot;, true);

            // Set the placement type of the chart
            chart.Placement = PlacementType.MoveAndSize;

            // Output the placement type
            Console.WriteLine(&quot;Chart Placement Type: &quot; + chart.Placement);

            // Save the workbook
            workbook.Save(&quot;PlacementTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


