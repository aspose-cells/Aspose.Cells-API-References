##Chart.BackWall
Chart property. Returns a Walls object that represents the back wall of a 3D chart
## Chart.BackWall property
Returns a [`Walls`](../walls/) object that represents the back wall of a 3-D chart.
```csharp
public Walls BackWall { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPropertyBackWallDemo
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
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["B3"].PutValue(1500);
worksheet.Cells["B4"].PutValue(1800);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", true);
// Make sure it's a 3D chart
if (chart.Is3D)
{
// Get the BackWall object
Walls backWall = chart.BackWall;
// Display some properties of the BackWall
Console.WriteLine("BackWall properties:");
Console.WriteLine("CenterX: " + backWall.CenterX);
Console.WriteLine("CenterY: " + backWall.CenterY);
Console.WriteLine("Width: " + backWall.Width);
Console.WriteLine("Height: " + backWall.Height);
// Format the BackWall
backWall.FillFormat.SetOneColorGradient(
System.Drawing.Color.LightBlue,
0.5, // Changed from GradientStyleType to double for degree parameter
Aspose.Cells.Drawing.GradientStyleType.Horizontal,
1); // Changed from 0.5 to int for variant parameter
// Set border properties
backWall.Border.Color = System.Drawing.Color.DarkBlue;
backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
}
// Save the workbook
workbook.Save("ChartPropertyBackWallDemo.xlsx");
}
}
}
```
### See Also
* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
