##Walls.GetCubePointCount
Walls method. Gets the number of cube points after calls Chart.Calculate method
## Walls.GetCubePointCount method
Gets the number of cube points after calls Chart.Calculate() method.
```csharp
public int GetCubePointCount()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class WallsMethodGetCubePointCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a 3D chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to ensure Wall properties are available
chart.Calculate();
try
{
// Get the Walls object
Walls walls = chart.Walls;
// Call the GetCubePointCount method
int pointCount = walls.GetCubePointCount();
// Display the result
Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
// Save the workbook
workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
}
}
}
}
```
### See Also
* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
