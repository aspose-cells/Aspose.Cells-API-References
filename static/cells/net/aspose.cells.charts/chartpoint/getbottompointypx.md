##ChartPoint.GetBottomPointYPx
ChartPoint method. Gets ycoordinate of the bottom point of shape after calls Chart.Calculate method. Applies 3D charts Column3D Bar3D Cone Cylinder Pyramid
## ChartPoint.GetBottomPointYPx method
Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid
```csharp
public float GetBottomPointYPx(int index)
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointMethodGetBottomPointYPxDemo
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
// Add series
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure all points are calculated
chart.Calculate();
// Get the first point of first series
ChartPoint point = chart.NSeries[0].Points[0];
try
{
// Get the number of bottom points
int bottomPointCount = point.GetBottomPointCount();
if (bottomPointCount > 0)
{
// Call GetBottomPointYPx with index 0
float yPx = point.GetBottomPointYPx(0);
Console.WriteLine($"Bottom point Y position in pixels: {yPx}");
Console.WriteLine("Method executed successfully with parameter (Int32)");
}
else
{
Console.WriteLine("No bottom points available for this chart point");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetBottomPointYPx method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetBottomPointYPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
