##Walls.DepthPx
Walls property. Gets the depth front to back in units of pixels after calls Chart.Calculate method
## Walls.DepthPx property
Gets the depth front to back in units of pixels after calls Chart.Calculate() method.
```csharp
public int DepthPx { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class WallsPropertyDepthPxDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Create 3D chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get walls and demonstrate DepthPx property
Walls walls = chart.Walls;
Console.WriteLine("Wall Depth in Pixels: " + walls.DepthPx);
// Save workbook
workbook.Save("WallsDepthPxDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
