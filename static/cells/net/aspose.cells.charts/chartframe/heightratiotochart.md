##ChartFrame.HeightRatioToChart
ChartFrame property. Gets or sets the height of frame in units of ratio of the chart area
## ChartFrame.HeightRatioToChart property
Gets or sets the height of frame in units of ratio of the chart area.
```csharp
public virtual double HeightRatioToChart { get; set; }
```
### Remarks
This is a fraction value, its valid range is between 0-1. How to convert units of ratio to pixels? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyHeightRatioToChartDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart title (which inherits from ChartFrame)
chart.Title.Text = "Sample Chart";
ChartFrame titleFrame = chart.Title;
// Display current HeightRatioToChart value
Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);
// Set a new height ratio (0.1 = 10% of chart height)
titleFrame.HeightRatioToChart = 0.1;
// Demonstrate the effect by comparing before/after
Console.WriteLine("Title height reduced to 10% of chart height");
// Save the result
workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
