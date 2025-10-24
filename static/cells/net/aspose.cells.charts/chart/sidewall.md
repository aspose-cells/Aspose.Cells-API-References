##Chart.SideWall
Chart property. Returns a Walls object that represents the side wall of a 3D chart
## Chart.SideWall property
Returns a [`Walls`](../walls/) object that represents the side wall of a 3-D chart.
```csharp
public Walls SideWall { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPropertySideWallDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["C2"].PutValue(150);
worksheet.Cells["C3"].PutValue(250);
worksheet.Cells["C4"].PutValue(350);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:C4", true);
// Access the SideWall property
Walls sideWall = chart.SideWall;
// Display some properties of the SideWall
Console.WriteLine("SideWall properties:");
Console.WriteLine("Width: " + sideWall.Width);
Console.WriteLine("Height: " + sideWall.Height);
Console.WriteLine("Depth: " + sideWall.Depth);
// Calculate the chart to update wall dimensions
chart.Calculate();
// Display updated properties after calculation
Console.WriteLine("\nAfter Calculate():");
Console.WriteLine("SideWall CenterX: " + sideWall.CenterX);
Console.WriteLine("SideWall CenterY: " + sideWall.CenterY);
Console.WriteLine("SideWall WidthPx: " + sideWall.WidthPx);
Console.WriteLine("SideWall HeightPx: " + sideWall.HeightPx);
// Save the workbook
workbook.Save("ChartPropertySideWallDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
