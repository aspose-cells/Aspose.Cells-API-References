##ChartPoint.InnerArcStartPointYPx
ChartPoint property. Gets the y coordinate of starting point for the pie section after calls Chart.Calculate method. Applies to Doughnut chart
## ChartPoint.InnerArcStartPointYPx property
Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```csharp
public float InnerArcStartPointYPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyInnerArcStartPointYPxDemo
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
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart to ensure properties are populated
chart.Calculate();
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the InnerArcStartPointYPx value
Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);
// Note: InnerArcStartPointYPx is read-only, so we can't set it directly
// To change the position, we need to adjust the doughnut hole size
chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size
// Recalculate the chart to update properties
chart.Calculate();
// Display the new InnerArcStartPointYPx value after changing hole size
Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);
// Save the workbook
workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
