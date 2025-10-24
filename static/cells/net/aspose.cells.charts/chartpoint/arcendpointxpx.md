##ChartPoint.ArcEndPointXPx
ChartPoint property. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate method. Applies to Pie and Doughnut chart
## ChartPoint.ArcEndPointXPx property
Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
```csharp
public float ArcEndPointXPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyArcEndPointXPxDemo
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
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure properties are populated
chart.Calculate();
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the ArcEndPointXPx value
Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);
// Note: ArcEndPointXPx is read-only, so we cannot set it directly
// To change the endpoint, we need to modify the chart data or properties that affect the pie slice
// Example of how changing data affects the ArcEndPointXPx
worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
chart.Calculate(); // Recalculate chart
// Display the new ArcEndPointXPx value after data change
Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);
// Save the workbook
workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
