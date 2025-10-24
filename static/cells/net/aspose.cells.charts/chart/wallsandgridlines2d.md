##Chart.WallsAndGridlines2D
Chart property. True if gridlines are drawn twodimensionally on a 3D chart
## Chart.WallsAndGridlines2D property
True if gridlines are drawn two-dimensionally on a 3-D chart.
```csharp
public bool WallsAndGridlines2D { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyWallsAndGridlines2DDemo
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
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["B4"].PutValue(15);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate WallsAndGridlines2D property
chart.WallsAndGridlines2D = true; // Show walls and gridlines in 2D
Console.WriteLine("WallsAndGridlines2D is set to: " + chart.WallsAndGridlines2D);
// Save the workbook
workbook.Save("WallsAndGridlines2DDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
