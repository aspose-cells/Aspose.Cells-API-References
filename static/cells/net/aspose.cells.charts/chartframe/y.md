##ChartFrame.Y
ChartFrame property. Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area
## ChartFrame.Y property
Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```
### Remarks
How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;
NOTE: This member is now obsolete. Please use ChartFrame.YRatioToChart property, instead. Y = YRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
Cells cells = sheet.Cells;
cells["A1"].PutValue("Category");
cells["A2"].PutValue("A");
cells["A3"].PutValue("B");
cells["A4"].PutValue("C");
cells["B1"].PutValue("Value");
cells["B2"].PutValue(10);
cells["B3"].PutValue(20);
cells["B4"].PutValue(30);
// Add chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Access chart title and set Y position
chart.Title.Text = "Sample Chart";
chart.Title.Y = 1000; // Demonstrate Y property usage
// Save the workbook
workbook.Save("ChartFramePropertyYDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
