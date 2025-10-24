##Title.XRatioToChart
Title property. Gets or sets the x coordinate of the upper left corner in units of Fraction of the chart area. X In Pixels  XRatioToChart  Chart.ChartObject.Width
## Title.XRatioToChart property
Gets or sets the x coordinate of the upper left corner in units of Fraction of the chart area. X In Pixels = XRatioToChart * Chart.ChartObject.Width;
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
public class TitlePropertyXRatioToChartDemo
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
// Set data source for the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the chart title
chart.Title.Text = "Sample Chart Title";
Title title = chart.Title;
// Display current XRatioToChart value
Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);
// Change the XRatioToChart value to move the title horizontally
title.XRatioToChart = 0.25; // 25% from the left of the chart area
Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);
// Save the workbook
workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
