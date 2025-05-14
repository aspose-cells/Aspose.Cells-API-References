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
public static void Chart_Property_Placement()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Set the chart data range
            chart.SetChartDataRange("A1:B4", true);

            // Set the placement type of the chart
            chart.Placement = PlacementType.MoveAndSize;

            // Output the placement type
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Save the workbook
            workbook.Save("PlacementTypeExample.xlsx");
        }
```

### See Also

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


