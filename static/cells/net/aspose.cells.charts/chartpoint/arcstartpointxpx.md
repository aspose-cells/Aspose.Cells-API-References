##ChartPoint.ArcStartPointXPx
ChartPoint property. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate method. Applies to Pie and Doughnut chart
## ChartPoint.ArcStartPointXPx property
Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
```csharp
public float ArcStartPointXPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyArcStartPointXPxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
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
// Display the ArcStartPointXPx value
Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);
// Note: ArcStartPointXPx is read-only, so we can't set it directly
// Instead, we can demonstrate how it changes when we modify other properties
// Change the explosion value which affects the pie slice position
point.Explosion = 20;
chart.Calculate(); // Recalculate to update properties
// Display the new ArcStartPointXPx value after explosion change
Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);
// Save the workbook
workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
