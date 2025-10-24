##ChartFrame.DefaultHeight
ChartFrame property. Represents height of default position in units of 1/4000 of the chart area
## ChartFrame.DefaultHeight property
Represents height of default position in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartFrame.DefaultHeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultHeight { get; }
```
### Remarks
NOTE: This member is now obsolete. Please use ChartFrame.DefaultHeightRatioToChart property, instead. DefaultHeight = (int)(DefaultHeightRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultHeightDemo
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
// Access the chart's title (which is a ChartFrame)
ChartFrame chartTitle = chart.Title;
// Display the current DefaultHeight value (read-only property)
Console.WriteLine("Current DefaultHeight value: " + chartTitle.DefaultHeight);
// Demonstrate how DefaultHeight affects the chart layout
Console.WriteLine("DefaultHeightRatioToChart: " + chartTitle.DefaultHeightRatioToChart);
Console.WriteLine("Current HeightRatioToChart: " + chartTitle.HeightRatioToChart);
// Adjust the height using the writable property
chartTitle.HeightRatioToChart = chartTitle.DefaultHeightRatioToChart * 1.5;
Console.WriteLine("New HeightRatioToChart: " + chartTitle.HeightRatioToChart);
// Save the result
workbook.Save("ChartFrameDefaultHeightDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
