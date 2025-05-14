---
title: ChartPoint.Border
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets the  border
type: docs
url: /net/aspose.cells.charts/chartpoint/border/
---
## ChartPoint.Border property

Gets the [` border`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: point.Border.Color = System.Drawing.Color.Red;
public static void ChartPoint_Property_Border()
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

            // Accessing the ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Iterating through the points in the collection
            for (int i = 0; i < points.Count; i++)
            {
                // Get Data Point
                ChartPoint point = points[i];
                
                // Set Pie Explosion
                point.Explosion = 15;
                
                // Set Border Color
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Saving the Excel file
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


