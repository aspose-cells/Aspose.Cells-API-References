##ChartPoint.InnerArcStartPointXPx
ChartPoint property. Gets the x coordinate of starting point for the pie section after calls Chart.Calculate method. Applies to Doughnut chart
## ChartPoint.InnerArcStartPointXPx property
Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.
```csharp
public float InnerArcStartPointXPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyInnerArcStartPointXPxDemo
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
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a doughnut chart
int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to get the shape properties
chart.Calculate();
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the InnerArcStartPointXPx value
Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);
// Note: InnerArcStartPointXPx is read-only, so we can't set it directly
// To change the position, we would need to modify the chart size or doughnut hole size
// Save the workbook
workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
