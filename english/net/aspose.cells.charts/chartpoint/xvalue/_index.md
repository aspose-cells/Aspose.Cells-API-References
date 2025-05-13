---
title: ChartPoint.XValue
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets or sets the X value of the chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

Gets or sets the X value of the chart point.

```csharp
public object XValue { get; set; }
```

### Examples

```csharp
// Called: point.XValue = "Category " + (i + 1);
public static void ChartPoint_Property_XValue()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding sample values to cells
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Adding a chart to the worksheet
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Accessing the instance of the newly added chart
            Chart chart = worksheet.Charts[chartIndex];

            // Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
            chart.NSeries.Add("A1:B3", true);

            // Show Data Labels
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Iterate through each point in the series
            for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
            {
                // Get Data Point
                ChartPoint point = chart.NSeries[0].Points[i];

                // Set Pie Explosion
                point.Explosion = 15;

                // Set Border Color
                point.Border.Color = Color.Red;

                // Set Shadow
                point.Shadow = true;

                // Set YValue
                point.YValue = 100 + i * 10;

                // Set XValue
                point.XValue = "Category " + (i + 1);

                // Set IsInSecondaryPlot
                point.IsInSecondaryPlot = false;
            }

            // Saving the Excel file
            workbook.Save("ChartPointExample.xlsx");
            workbook.Save("ChartPointExample.pdf");
        }
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


