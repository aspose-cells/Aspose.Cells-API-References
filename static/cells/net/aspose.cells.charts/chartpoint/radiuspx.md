##ChartPoint.RadiusPx
ChartPoint property. Gets the radius of bubble pie or doughnut in units of pixels after calls Chart.Calculate method
## ChartPoint.RadiusPx property
Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.
```csharp
public int RadiusPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyRadiusPxDemo
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
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure properties are populated
chart.Calculate();
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current radius value
Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);
// Note: RadiusPx is read-only, so we can't set it directly
// To change the radius, we need to adjust the chart size or other properties
// that affect the point size indirectly
// Example of how changing chart size affects radius
Console.WriteLine("\nChanging chart size to demonstrate radius change...");
chart.ChartObject.Width = 800;
chart.ChartObject.Height = 600;
chart.Calculate();
// Display the new radius value after chart resize
Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);
// Save the result
workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
