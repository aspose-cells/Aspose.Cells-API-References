##Title.YRatioToChart
Title property. Gets or sets the y coordinate of the upper left corner in units of Fraction of the chart area. Y In Pixels  YRatioToChart  Chart.ChartObject.Width
## Title.YRatioToChart property
Gets or sets the y coordinate of the upper left corner in units of Fraction of the chart area. Y In Pixels = YRatioToChart * Chart.ChartObject.Width;
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
public class TitlePropertyYRatioToChartDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the chart title
chart.Title.Text = "Sample Chart Title";
Title chartTitle = chart.Title;
// Display current YRatioToChart value
Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);
// Change the YRatioToChart property to move the title vertically
chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);
// Save the workbook
workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
