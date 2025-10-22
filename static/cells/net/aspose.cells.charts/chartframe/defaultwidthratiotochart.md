##ChartFrame.DefaultWidthRatioToChart
ChartFrame property. Represents width of default position in units of Fraction of the chart area
## ChartFrame.DefaultWidthRatioToChart property
Represents width of default position in units of Fraction of the chart area.
```csharp
public double DefaultWidthRatioToChart { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultWidthRatioToChartDemo
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
// Access the chart's title which is a ChartFrame
ChartFrame chartTitle = chart.Title;
// Display the current DefaultWidthRatioToChart value
Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);
// Note: DefaultWidthRatioToChart is read-only, so we can't set it
// Instead, we'll demonstrate its relationship with the actual width ratio
Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);
// Change the width ratio to demonstrate its effect
chartTitle.WidthRatioToChart = 0.5;
Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);
// Save the workbook
workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
