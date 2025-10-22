##ChartPoint.ArcStartPointYPx
ChartPoint property. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate method. Applies to Pie and Doughnut chart
## ChartPoint.ArcStartPointYPx property
Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
```csharp
public float ArcStartPointYPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyArcStartPointYPxDemo
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
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to get the shape positions
chart.Calculate();
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current ArcStartPointYPx value
Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);
// Note: ArcStartPointYPx is read-only, so we can't set it directly
// Instead, we'll demonstrate how changing other properties affects ArcStartPointYPx
// Change the explosion value to modify the pie slice position
point.Explosion = 20;
// Recalculate the chart to update positions
chart.Calculate();
// Display the new ArcStartPointYPx value after changing explosion
Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);
// Save the workbook
workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
