##ChartPoint.DoughnutInnerRadius
ChartPoint property. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate method. Applies to Doughnut chart
## ChartPoint.DoughnutInnerRadius property
Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.
```csharp
public int DoughnutInnerRadius { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyDoughnutInnerRadiusDemo
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
worksheet.Cells["B2"].PutValue(4);
worksheet.Cells["B3"].PutValue(3);
worksheet.Cells["B4"].PutValue(5);
// Add a doughnut chart
int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to get the chart points
chart.Calculate();
// Get the first chart point from the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current DoughnutInnerRadius value
Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);
// Note: DoughnutInnerRadius is read-only, so we can't set it directly
// To change the inner radius, we need to adjust the HoleSize property of the chart
chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available
// Recalculate the chart to update the DoughnutInnerRadius
chart.Calculate();
// Display the updated DoughnutInnerRadius value
Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);
// Save the workbook
workbook.Save("DoughnutInnerRadiusDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
