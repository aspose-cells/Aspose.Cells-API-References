---
title: ChartFrame.Y
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.YRatioToChart property, instead. Y = YRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: legend.Y = 1500;
public static void Property_Y()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Add a column chart to the worksheet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Access the legend of the chart
            Legend legend = chart.Legend;

            // Set the legend's position to the left of the chart
            legend.Position = LegendPositionType.Left;

            // Set additional properties for the legend
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Save the workbook
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


