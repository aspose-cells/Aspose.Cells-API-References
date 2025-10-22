##Walls.GetCubePointYPx
Walls method. Gets ycoordinate of the apex point of walls cube after calls Chart.Calculate method. The number of apex points of walls cube is eight
## Walls.GetCubePointYPx method
Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight.
```csharp
public float GetCubePointYPx(int index)
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class WallsMethodGetCubePointYPxDemo
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
// Add a 3D chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to ensure Wall properties are populated
chart.Calculate();
// Get the Walls object
Walls walls = chart.Walls;
try
{
// Get the number of cube points
int pointCount = walls.GetCubePointCount();
if (pointCount > 0)
{
// Call GetCubePointYPx with the first index (0)
float yPx = walls.GetCubePointYPx(0);
Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
}
else
{
Console.WriteLine("No cube points available in the walls.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
}
// Save the workbook
workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
