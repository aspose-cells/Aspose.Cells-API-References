##ChartPoint.GetTopPointXPx
ChartPoint method. Gets xcoordinate of the top point of shape after calls Chart.Calculate method. Applies 3D charts Column3D Bar3D Cone Cylinder Pyramid and Area3D
## ChartPoint.GetTopPointXPx method
Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D
```csharp
public float GetTopPointXPx(int index)
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointMethodGetTopPointXPxWithInt32Demo
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure all position properties are calculated
chart.Calculate();
try
{
// Get the first chart point from first series
ChartPoint point = chart.NSeries[0].Points[0];
// Get the number of top points
int pointCount = point.GetTopPointCount();
if (pointCount > 0)
{
// Call GetTopPointXPx with index 0
float xPos = point.GetTopPointXPx(0);
Console.WriteLine($"X position of top point (pixels): {xPos}");
}
else
{
Console.WriteLine("No top points available for this chart point");
}
Console.WriteLine("Method executed successfully with parameters (Int32)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTopPointXPx method: {ex.Message}");
}
// Save the result
workbook.Save("ChartPointMethodGetTopPointXPxWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
