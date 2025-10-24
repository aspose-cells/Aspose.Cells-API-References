##Chart.Walls
Chart property. Returns a Walls object that represents the walls of a 3D chart
## Chart.Walls property
Returns a `Walls` object that represents the walls of a 3-D chart.
```csharp
public Walls Walls { get; }
```
### Remarks
This property doesn't apply to 3-D pie charts.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartPropertyWallsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(35);
// Create cylinder column chart
int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Configure chart basics
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
chart.IsRectangularCornered = true;
chart.RotationAngle = 20;
// Configure walls properties
Walls walls = chart.Walls;
walls.BackgroundColor = Color.LightGray;
walls.ForegroundColor = Color.Transparent;
walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);
// Save the result
workbook.Save("ChartWallsDemo_out.xlsx");
}
}
}
```
### See Also
* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
