##ChartArea.HeightRatioToChart
ChartArea property. Gets or sets the vertical offset from its lower right corner row in units of ratio of the chart area
## ChartArea.HeightRatioToChart property
Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area.
```csharp
public override double HeightRatioToChart { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartAreaPropertyHeightRatioToChartDemo
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
// Access the chart area
ChartArea chartArea = chart.ChartArea;
// Display the current HeightRatioToChart value
Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);
// Set a new value for HeightRatioToChart (0.5 = 50% of chart height)
chartArea.HeightRatioToChart = 0.5;
Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);
// Set a new value for WidthRatioToChart to demonstrate combined effect
chartArea.WidthRatioToChart = 0.8;
// Save the workbook to see the changes
workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
