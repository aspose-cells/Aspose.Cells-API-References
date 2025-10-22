##Chart.PlotVisibleCells
Chart property. Indicates whether only plot visible cells
## Chart.PlotVisibleCells property
Indicates whether only plot visible cells.
```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyPlotVisibleCellsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("Alice");
worksheet.Cells["A3"].PutValue("Bob");
worksheet.Cells["A4"].PutValue("Eve");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["B2"].PutValue(90);
worksheet.Cells["B3"].PutValue(85);
worksheet.Cells["B4"].PutValue(95);
// Hide some rows
worksheet.Cells.HideRow(2);
worksheet.Cells.HideRow(3);
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate PlotVisibleCells property
chart.PlotVisibleCells = false; // Will not plot hidden cells
// chart.PlotVisibleCells = true; // Will plot hidden cells (commented out for demo)
// Save the workbook
workbook.Save("ChartPlotVisibleCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
