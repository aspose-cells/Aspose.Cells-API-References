##ChartPoint.EndAngle
ChartPoint property. Gets the ending angle for the pie section measured in degrees clockwise from the xaxis after calls Chart.Calculate method. Applies to Pie chart
## ChartPoint.EndAngle property
Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.
```csharp
public float EndAngle { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyEndAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pie chart
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure properties are populated
chart.Calculate();
// Get the first chart point (Apple slice)
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current EndAngle value
Console.WriteLine("Current EndAngle value: " + point.EndAngle);
// Note: EndAngle is read-only, so we can't set it directly
// Instead, we'll demonstrate how it relates to the pie slice
// Explode the point to see how it affects the angles
point.Explosion = 20;
chart.Calculate(); // Recalculate to update angles
// Display the new EndAngle after explosion
Console.WriteLine("EndAngle after explosion: " + point.EndAngle);
// Save the workbook
workbook.Save("ChartPointEndAngleDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
