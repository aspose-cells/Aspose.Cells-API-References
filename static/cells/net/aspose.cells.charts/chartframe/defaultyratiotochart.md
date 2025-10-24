##ChartFrame.DefaultYRatioToChart
ChartFrame property. Represents y of default position in units of Fraction of the chart area
## ChartFrame.DefaultYRatioToChart property
Represents y of default position in units of Fraction of the chart area.
```csharp
public double DefaultYRatioToChart { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultYRatioToChartDemo
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
// Add a chart and get its chart frame
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Get the chart frame (title in this case)
ChartFrame chartFrame = chart.Title;
// Display the current DefaultYRatioToChart value
Console.WriteLine("Current DefaultYRatioToChart value: " + chartFrame.DefaultYRatioToChart);
// Demonstrate how changing YRatioToChart affects position (since DefaultYRatioToChart is read-only)
Console.WriteLine("Current YRatioToChart value: " + chartFrame.YRatioToChart);
chartFrame.YRatioToChart = 0.1; // Move title up
Console.WriteLine("New YRatioToChart value: " + chartFrame.YRatioToChart);
// Save the result
workbook.Save("PropertyDefaultYRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
