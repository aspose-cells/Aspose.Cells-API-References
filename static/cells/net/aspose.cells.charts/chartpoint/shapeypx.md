##ChartPoint.ShapeYPx
ChartPoint property. Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate method
## ChartPoint.ShapeYPx property
Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.
```csharp
public int ShapeYPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyShapeYPxDemo
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
// Calculate chart to get shape positions
chart.Calculate();
// Get first point in first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display current Y position in pixels
Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);
// Note: ShapeYPx is read-only, so we can't set it directly
// To change position, we need to modify the chart size/position or data
// Demonstrate effect by changing chart position which will affect point positions
chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
chart.Calculate(); // Recalculate to update positions
// Show new Y position after chart movement
Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);
// Save the result
workbook.Save("ChartPointShapeYPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
