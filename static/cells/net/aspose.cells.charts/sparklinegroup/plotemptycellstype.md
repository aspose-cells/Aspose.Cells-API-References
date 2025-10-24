##SparklineGroup.PlotEmptyCellsType
SparklineGroup property. Indicates how to plot empty cells
## SparklineGroup.PlotEmptyCellsType property
Indicates how to plot empty cells.
```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add data with some empty cells
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(null); // Empty cell
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
// Define the CellArea for the sparkline
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add a sparkline group
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Set how empty cells should be plotted
group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
// Add sparkline to the group
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Save the workbook
workbook.Save("SparklineEmptyCellsDemo.xlsx");
}
}
}
```
### See Also
* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
