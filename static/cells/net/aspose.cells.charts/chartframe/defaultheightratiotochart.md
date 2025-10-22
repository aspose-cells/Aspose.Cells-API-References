##ChartFrame.DefaultHeightRatioToChart
ChartFrame property. Represents height of default position in units of Fraction of the chart area
## ChartFrame.DefaultHeightRatioToChart property
Represents height of default position in units of Fraction of the chart area.
```csharp
public double DefaultHeightRatioToChart { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultHeightRatioToChartDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart title (which is a ChartFrame)
ChartFrame chartTitle = chart.Title;
// Display the current DefaultHeightRatioToChart value
Console.WriteLine("Current DefaultHeightRatioToChart value: " + chartTitle.DefaultHeightRatioToChart);
// Demonstrate how this property affects the chart by comparing with HeightRatioToChart
Console.WriteLine("Current HeightRatioToChart value: " + chartTitle.HeightRatioToChart);
// Change the height ratio to see the effect
chartTitle.HeightRatioToChart = 0.1;
Console.WriteLine("After setting HeightRatioToChart to 0.1: " + chartTitle.HeightRatioToChart);
// Save the workbook
workbook.Save("ChartFramePropertyDefaultHeightRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
