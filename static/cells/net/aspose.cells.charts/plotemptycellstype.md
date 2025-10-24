##Enum PlotEmptyCellsType
Aspose.Cells.Charts.PlotEmptyCellsType enum. Represents all plot empty cells type of a chart
## PlotEmptyCellsType enumeration
Represents all plot empty cells type of a chart.
```csharp
public enum PlotEmptyCellsType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| NotPlotted | `0` | Not plotted(leave gap) |
| Zero | `1` | Zero |
| Interpolated | `2` | Interpolated |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class PlotEmptyCellsTypeDemo
{
public static void PlotEmptyCellsTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(null); // Empty cell
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B5"].PutValue(40);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set the data range for the chart
chart.SetChartDataRange("A1:B5", true);
// Set the title of the chart
chart.Title.Text = "Plot Empty Cells Example";
// Set how to plot empty cells
chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;
// Save the workbook
workbook.Save("PlotEmptyCellsTypeExample.xlsx");
Console.WriteLine("Workbook saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
