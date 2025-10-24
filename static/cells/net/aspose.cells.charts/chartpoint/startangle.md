##ChartPoint.StartAngle
ChartPoint property. Gets the starting angle for the pie section measured in degrees clockwise from the xaxis after calls Chart.Calculate method. Applies to Pie chart
## ChartPoint.StartAngle property
Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.
```csharp
public float StartAngle { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyStartAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
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
// Display the StartAngle value
Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);
// Note: StartAngle is read-only, so we can't set it directly
// To change the start angle, we need to rotate the entire pie chart
chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees
// Recalculate to update angles
chart.Calculate();
// Display the new StartAngle value after rotation
Console.WriteLine("StartAngle after rotation: " + point.StartAngle);
// Save the workbook
workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
