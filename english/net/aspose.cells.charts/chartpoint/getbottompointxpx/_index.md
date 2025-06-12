---
title: ChartPoint.GetBottomPointXPx
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint method. Gets xcoordinate of the bottom point of shape after calls Chart.Calculate method. Applies 3D charts Column3D Bar3D Cone Cylinder Pyramid
type: docs
url: /net/aspose.cells.charts/chartpoint/getbottompointxpx/
---
## ChartPoint.GetBottomPointXPx method

Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

```csharp
public float GetBottomPointXPx(int index)
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a column chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculate chart to ensure all position properties are set
            chart.Calculate();

            try
            {
                // Get the first chart point from first series
                ChartPoint point = chart.NSeries[0].Points[0];

                // Get the number of bottom points
                int bottomPointCount = point.GetBottomPointCount();

                if (bottomPointCount > 0)
                {
                    // Call GetBottomPointXPx with index 0
                    float xPos = point.GetBottomPointXPx(0);
                    Console.WriteLine($"X position of bottom point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointXPx method: {ex.Message}");
            }

            // Save the result
            workbook.Save("ChartPointMethodGetBottomPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


