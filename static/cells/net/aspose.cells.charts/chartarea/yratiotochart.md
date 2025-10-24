##ChartArea.YRatioToChart
ChartArea property. Gets or gets the vertical offset from its upper left corner row in units of ratio of the chart area
## ChartArea.YRatioToChart property
Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area.
```csharp
public override double YRatioToChart { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartAreaPropertyYRatioToChartDemo
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
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart area
ChartArea chartArea = chart.ChartArea;
// Display the current YRatioToChart value
Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);
// Change the YRatioToChart property (0.0 to 1.0 represents 0% to 100% of chart area)
chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height
// Display the new YRatioToChart value
Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);
// Save the workbook to see the effect
workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
