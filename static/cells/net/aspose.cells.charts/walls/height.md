##Walls.Height
Walls property. Gets the height of top to bottom in units of 1/4000 of charts height after calls Chart.Calculate method
## Walls.Height property
Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```csharp
public int Height { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class WallsPropertyHeightDemo
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
// Add 3D chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
chart.Calculate();
// Access walls and demonstrate Height property
Walls walls = chart.Walls;
Console.WriteLine("Wall Height: " + walls.Height);
Console.WriteLine("Wall Height in Pixels: " + walls.HeightPx);
// Modify chart area size instead of direct Height property
chart.ChartObject.Height = 400;
chart.Calculate();
Console.WriteLine("After resizing - Wall Height: " + walls.Height);
Console.WriteLine("After resizing - Wall Height in Pixels: " + walls.HeightPx);
workbook.Save("WallsHeightDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
