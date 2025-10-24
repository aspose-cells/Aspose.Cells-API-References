##ChartFrame.X
ChartFrame property. Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area
## ChartFrame.X property
Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```
### Remarks
How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;
NOTE: This member is now obsolete. Please use ChartFrame.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyXDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X Values");
sheet.Cells["B1"].PutValue("Y Values");
for (int i = 2; i <= 10; i++)
{
sheet.Cells["A" + i].PutValue(i);
sheet.Cells["B" + i].PutValue(i * 2);
}
// Add chart
int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Add series and set X/Y values
chart.NSeries.Add("Sheet1!B2:B10", true);
chart.NSeries[0].XValues = "Sheet1!A2:A10";
// Add trendline
chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
Trendline trendline = chart.NSeries[0].TrendLines[0];
// Configure data labels
trendline.DataLabels.ShowValue = true;
trendline.DataLabels.Font.Color = Color.Blue;
// Demonstrate X property usage
trendline.DataLabels.X = -500; // Set X position offset
trendline.DataLabels.Y = 200;  // Set Y position offset
// Save the workbook
workbook.Save("ChartFramePropertyXDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
