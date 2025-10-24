##Chart.Perspective
Chart property. Returns or sets the perspective for the 3D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True
## Chart.Perspective property
Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True.
```csharp
public short Perspective { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyPerspectiveDemo
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
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set 3D chart perspective properties
chart.Perspective = 30; // Perspective angle (0-100)
chart.RotationAngle = 15; // Rotation angle
chart.Elevation = 20; // Elevation angle
chart.RightAngleAxes = false; // Enable perspective projection
chart.AutoScaling = true; // Auto scale the chart
// Save the workbook
workbook.Save("ChartPerspectiveDemo.xlsx");
Console.WriteLine("Chart with perspective settings created successfully.");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
