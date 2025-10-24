##ChartPoint.InnerRadiusPx
ChartPoint property. Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate method. Applies to Doughnut chart
## ChartPoint.InnerRadiusPx property
Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.
```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ChartPoint.DoughnutInnerRadius property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyInnerRadiusPxDemo
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
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to get chart point properties
chart.Calculate();
// Get the first chart point from the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current inner radius value (read-only property)
Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);
// Note: InnerRadiusPx is read-only, so we cannot set it directly
// To change the inner radius, we need to adjust the doughnut hole size
chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size
// Recalculate the chart to update properties
chart.Calculate();
// Display the new inner radius value after changing doughnut hole size
Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);
// Save the result
workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
