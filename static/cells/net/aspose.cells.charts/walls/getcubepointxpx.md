##Walls.GetCubePointXPx
Walls method. Gets xcoordinate of the apex point of walls cube after calls Chart.Calculate method. The number of apex points of walls cube is eight
## Walls.GetCubePointXPx method
Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight
```csharp
public float GetCubePointXPx(int index)
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class WallsMethodGetCubePointXPxWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["A5"].PutValue("Q4");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
worksheet.Cells["B5"].PutValue(4000);
// Create a 3D chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Calculate the chart to ensure Wall properties are available
chart.Calculate();
// Get the Walls object
Walls walls = chart.Walls;
try
{
// Get the cube point count
int pointCount = walls.GetCubePointCount();
if (pointCount > 0)
{
// Call GetCubePointXPx with index 0 (first point)
float xCoordinate = walls.GetCubePointXPx(0);
Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
Console.WriteLine("Method executed successfully with parameter (Int32)");
}
else
{
Console.WriteLine("No cube points available in the walls");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
}
// Save the workbook
workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
