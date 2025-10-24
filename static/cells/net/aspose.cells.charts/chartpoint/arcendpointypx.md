##ChartPoint.ArcEndPointYPx
ChartPoint property. Gets the y coordinate of ending point for the pie section after calls Chart.Calculate method. Applies to Pie and Doughnut chart
## ChartPoint.ArcEndPointYPx property
Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.
```csharp
public float ArcEndPointYPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyArcEndPointYPxDemo
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
worksheet.Cells["B2"].PutValue(8000);
worksheet.Cells["B3"].PutValue(12000);
worksheet.Cells["B4"].PutValue(14000);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to get the shape positions
chart.Calculate();
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current ArcEndPointYPx value
Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);
// Since ArcEndPointYPx is read-only, we can only read it
// The following line would cause a compilation error:
// point.ArcEndPointYPx = 150.5f;
// Demonstrate how this property affects the pie chart
Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");
// Save the workbook
workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
