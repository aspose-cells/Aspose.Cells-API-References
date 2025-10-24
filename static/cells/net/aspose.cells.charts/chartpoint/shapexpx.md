##ChartPoint.ShapeXPx
ChartPoint property. Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate method
## ChartPoint.ShapeXPx property
Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.
```csharp
public int ShapeXPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeXPxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
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
// Calculate the chart to get shape positions
chart.Calculate();
// Get the first chart point from the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current X position in pixels
Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);
// Note: ShapeXPx is read-only, so we can't set it directly
// To change position, we would need to modify the chart size/position or data
// Demonstrate how the property changes when we modify the chart
Console.WriteLine("\nChanging chart position...");
chart.ChartObject.Left = 3;
chart.ChartObject.Top = 2;
chart.Calculate(); // Recalculate to update positions
Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);
// Save the result
workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
