##ChartPoint.InnerArcEndPointXPx
ChartPoint property. Gets the x coordinate of ending point for the pie section after calls Chart.Calculate method. Applies to Doughnut chart
## ChartPoint.InnerArcEndPointXPx property
Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```csharp
public float InnerArcEndPointXPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyInnerArcEndPointXPxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("C1");
worksheet.Cells["A3"].PutValue("C2");
worksheet.Cells["A4"].PutValue("C3");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(5);
worksheet.Cells["B3"].PutValue(3);
worksheet.Cells["B4"].PutValue(2);
// Add a doughnut chart
int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to get the chart point properties
chart.Calculate();
// Get the first chart point from the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current InnerArcEndPointXPx value
Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);
// Note: InnerArcEndPointXPx is read-only, so we can't set it directly
// To change the endpoint position, we need to modify the doughnut hole size
chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%
// Recalculate the chart to update the properties
chart.Calculate();
// Display the new InnerArcEndPointXPx value after changing the hole size
Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);
// Save the workbook
workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
