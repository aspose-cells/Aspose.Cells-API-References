##ChartArea.XRatioToChart
ChartArea property. Gets or gets the horizontal offset from its upper left corner column in units of ratio of the chart area
## ChartArea.XRatioToChart property
Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area.
```csharp
public override double XRatioToChart { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartAreaPropertyXRatioToChartDemo
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
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Get the chart area
ChartArea chartArea = chart.ChartArea;
// Display the current XRatioToChart value
Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);
// Change the XRatioToChart value to move the chart area horizontally
chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container
// Display the new XRatioToChart value
Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);
// Save the workbook
workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
