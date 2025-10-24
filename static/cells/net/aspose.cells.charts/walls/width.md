##Walls.Width
Walls property. Gets the width of left to right in units of 1/4000 of charts width after calls Chart.Calculate method
## Walls.Width property
Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```csharp
public int Width { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class WallsPropertyWidthDemo
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
// Add a 3D chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart
chart.Calculate();
// Access walls and demonstrate Width property
Aspose.Cells.Charts.Walls walls = chart.Walls;
Console.WriteLine("Wall Width: " + walls.Width);
Console.WriteLine("Wall Width in Pixels: " + walls.WidthPx);
// Save the workbook
workbook.Save("WallsWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
