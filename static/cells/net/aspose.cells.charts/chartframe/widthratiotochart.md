##ChartFrame.WidthRatioToChart
ChartFrame property. Gets or sets the width of frame in units of ratio of the chart area
## ChartFrame.WidthRatioToChart property
Gets or sets the width of frame in units of ratio of the chart area.
```csharp
public virtual double WidthRatioToChart { get; set; }
```
### Remarks
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyWidthRatioToChartDemo
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
// Access the chart title which is a ChartFrame
ChartFrame chartTitle = chart.Title;
// Display the current width ratio
Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);
// Set a new width ratio (0.5 = 50% of chart width)
chartTitle.WidthRatioToChart = 0.5;
// Show the effect by saving the workbook
workbook.Save("ChartFrameWidthRatioDemo.xlsx");
Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
