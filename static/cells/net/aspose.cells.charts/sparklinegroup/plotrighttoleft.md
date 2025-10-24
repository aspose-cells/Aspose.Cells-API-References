##SparklineGroup.PlotRightToLeft
SparklineGroup property. Indicates whether the plot data is right to left
## SparklineGroup.PlotRightToLeft property
Indicates whether the plot data is right to left.
```csharp
public bool PlotRightToLeft { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyPlotRightToLeftDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
// Create sparkline group
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 4;
ca.EndColumn = 4;
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Add sparkline
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Set sparkline colors
CellsColor seriesColor = workbook.CreateCellsColor();
seriesColor.Color = Color.Orange;
group.SeriesColor = seriesColor;
// Demonstrate PlotRightToLeft property
group.PlotRightToLeft = true; // Plot data points from right to left
// Save the workbook
workbook.Save("SparklineRightToLeftDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
