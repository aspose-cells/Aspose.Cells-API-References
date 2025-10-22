##ChartFrame.SetPositionAuto
ChartFrame method. Set position of the frame to automatic
## ChartFrame.SetPositionAuto method
Set position of the frame to automatic
```csharp
public virtual void SetPositionAuto()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFrameMethodSetPositionAutoDemo
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
// Get the chart title frame
ChartFrame title = chart.Title;
// Set manual position first to demonstrate SetPositionAuto
title.XRatioToChart = 0.2;
title.YRatioToChart = 0.1;
title.WidthRatioToChart = 0.6;
title.HeightRatioToChart = 0.1;
try
{
// Call the SetPositionAuto method
title.SetPositionAuto();
Console.WriteLine("Chart title position set to automatic successfully");
// Display the new automatic position values
Console.WriteLine($"New X position ratio: {title.XRatioToChart}");
Console.WriteLine($"New Y position ratio: {title.YRatioToChart}");
Console.WriteLine($"New Width ratio: {title.WidthRatioToChart}");
Console.WriteLine($"New Height ratio: {title.HeightRatioToChart}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetPositionAuto method: {ex.Message}");
}
// Save the result
workbook.Save("ChartFrameSetPositionAutoDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
