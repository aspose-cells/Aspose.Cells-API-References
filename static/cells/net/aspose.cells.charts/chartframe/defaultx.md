##ChartFrame.DefaultX
ChartFrame property. Represents x of default position in units of 1/4000 of the chart area
## ChartFrame.DefaultX property
Represents x of default position in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```
### Remarks
NOTE: This member is now obsolete. Please use ChartFrame.DefaultXRatioToChart property, instead. DefaultX = (int)(DefaultXRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultXDemo
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
// Access the chart title which inherits from ChartFrame
chart.Title.Text = "Sample Chart";
// Display the default X position of the chart title
Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
// Demonstrate how the default position affects the chart
Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
// Change the title's position using ratio properties (since DefaultX is read-only)
chart.Title.XRatioToChart = 0.2;
chart.Title.YRatioToChart = 0.05;
// Save the workbook
workbook.Save("ChartFrameDefaultXDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
