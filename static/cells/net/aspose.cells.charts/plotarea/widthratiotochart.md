##PlotArea.WidthRatioToChart
PlotArea property. Gets or sets the width of plotarea bounding box in units of ratio of the chart area
## PlotArea.WidthRatioToChart property
Gets or sets the width of plot-area bounding box in units of ratio of the chart area.
```csharp
public override double WidthRatioToChart { get; set; }
```
### Remarks
The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.
The **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** and **HeightRatioToChart** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.
For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().
WidthPixel = WidthRatioToChart * chart.ChartObject.Width.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class PlotAreaPropertyWidthRatioToChartDemo
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
// Add a chart and get its plot area
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
PlotArea plotArea = chart.PlotArea;
// Display current WidthRatioToChart value
Console.WriteLine("Current WidthRatioToChart value: " + plotArea.WidthRatioToChart);
// Change the width ratio and see the effect
plotArea.WidthRatioToChart = 0.6; // 60% of chart width
Console.WriteLine("WidthRatioToChart changed to: " + plotArea.WidthRatioToChart);
// Save the workbook
workbook.Save("PlotAreaWidthRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
