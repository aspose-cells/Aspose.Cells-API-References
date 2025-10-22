##ChartFrame.YRatioToChart
ChartFrame property. Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area
## ChartFrame.YRatioToChart property
Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area.
```csharp
public virtual double YRatioToChart { get; set; }
```
### Remarks
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? YPixel = YRatioToChart * Chart.ChartObject.Height;
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyYRatioToChartDemo
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
// Access the chart title which inherits from ChartFrame
chart.Title.Text = "Sample Chart";
// Display current YRatioToChart value
Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
// Change the Y position of the title relative to chart area
chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
// Display new YRatioToChart value
Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
// Access the legend which also inherits from ChartFrame
chart.Legend.Position = LegendPositionType.Top;
// Display current YRatioToChart value for legend
Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
// Change the Y position of the legend relative to chart area
chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
// Display new YRatioToChart value for legend
Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
// Save the workbook
workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
