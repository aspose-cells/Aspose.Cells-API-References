##Chart.PlotEmptyCellsType
Chart property. Gets and sets how to plot the empty cells
## Chart.PlotEmptyCellsType property
Gets and sets how to plot the empty cells.
```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyPlotEmptyCellsTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data with some empty cells
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["A3"].PutValue("B");
// B3 is left empty
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B4"].PutValue(30);
// Add chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate PlotEmptyCellsType property
chart.PlotEmptyCellsType = Aspose.Cells.Charts.PlotEmptyCellsType.Zero;
Console.WriteLine("PlotEmptyCellsType set to: " + chart.PlotEmptyCellsType);
// Save the workbook
workbook.Save("PlotEmptyCellsTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
