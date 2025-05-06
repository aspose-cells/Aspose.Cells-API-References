---
title: Axis.TickLabelPosition
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the position of tickmark labels on the specified axis
type: docs
url: /net/aspose.cells.charts/axis/ticklabelposition/
---
## Axis.TickLabelPosition property

Represents the position of tick-mark labels on the specified axis.

```csharp
public TickLabelPositionType TickLabelPosition { get; set; }
```

### Examples

```csharp
// Called: categoryAxis.TickLabelPosition = TickLabelPositionType.High;
public static void Property_TickLabelPosition()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add some sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(50);
            worksheet.Cells[&quot;A2&quot;].PutValue(100);
            worksheet.Cells[&quot;A3&quot;].PutValue(150);
            worksheet.Cells[&quot;B1&quot;].PutValue(4);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(50);
            
            // Add a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Add NSeries (chart data source) to the chart ranging from &quot;A1&quot; cell to &quot;B3&quot;
            chart.NSeries.Add(&quot;A1:B3&quot;, true);
            
            // Access the category axis
            Axis categoryAxis = chart.CategoryAxis;
            
            // Set the tick label position to High
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Save the workbook
            workbook.Save(&quot;TickLabelPositionTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


