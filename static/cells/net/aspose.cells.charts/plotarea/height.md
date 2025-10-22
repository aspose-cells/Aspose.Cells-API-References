##PlotArea.Height
PlotArea property. Gets or sets the height of plotarea bounding box in units of 1/4000 of the chart area
## PlotArea.Height property
Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use PlotArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```
### Remarks
The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.
The **X**, **Y**, **Width** and **Height** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.
For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().
NOTE: This member is now obsolete. Please use PlotArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class PlotAreaPropertyHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart
chart.Calculate();
// Demonstrate Height property
Console.WriteLine("Chart Area Height: " + chart.ChartArea.Height);
Console.WriteLine("Plot Area Height: " + chart.PlotArea.Height);
// Modify PlotArea height
chart.PlotArea.Height = 2500;
Console.WriteLine("Modified Plot Area Height: " + chart.PlotArea.Height);
}
}
}
```
### See Also
* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
