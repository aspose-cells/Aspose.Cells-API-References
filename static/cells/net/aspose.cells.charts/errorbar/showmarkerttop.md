##ErrorBar.ShowMarkerTTop
ErrorBar property. Indicates if formatting error bars with a Ttop
## ErrorBar.ShowMarkerTTop property
Indicates if formatting error bars with a T-top.
```csharp
public bool ShowMarkerTTop { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ErrorBarPropertyShowMarkerTTopDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].PutValue(10);
cells["A2"].PutValue(20);
cells["A3"].PutValue(30);
cells["B1"].PutValue(2);
cells["B2"].PutValue(3);
cells["B3"].PutValue(1);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("A1:A3", true);
chart.NSeries.CategoryData = "B1:B3";
// Configure error bars for the first series
Series series = chart.NSeries[0];
series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
series.YErrorBar.Type = ErrorBarType.Percent;
series.YErrorBar.Amount = 10;
// Demonstrate ShowMarkerTTop property
series.YErrorBar.ShowMarkerTTop = true;
series.YErrorBar.Color = System.Drawing.Color.Red;
series.YErrorBar.Style = LineType.DashDot;
// Save the workbook
workbook.Save("ErrorBarShowMarkerTTopDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
