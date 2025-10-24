##PlotArea.SetPositionAuto
PlotArea method. Set position of the plot area to automatic
## PlotArea.SetPositionAuto method
Set position of the plot area to automatic
```csharp
public override void SetPositionAuto()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class PlotAreaMethodSetPositionAutoDemo
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
try
{
// Get the plot area of the chart
PlotArea plotArea = chart.PlotArea;
// Manually set some position values first to demonstrate the effect
plotArea.XRatioToChart = 0.1;
plotArea.YRatioToChart = 0.1;
plotArea.WidthRatioToChart = 0.8;
plotArea.HeightRatioToChart = 0.8;
// Call SetPositionAuto to reset to automatic positioning
plotArea.SetPositionAuto();
Console.WriteLine("Plot area position has been set to automatic.");
// Save the workbook to show the effect
workbook.Save("PlotAreaSetPositionAutoDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
}
}
}
}
```
### See Also
* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
