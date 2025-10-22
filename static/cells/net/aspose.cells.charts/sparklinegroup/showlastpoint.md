##SparklineGroup.ShowLastPoint
SparklineGroup property. Indicates whether to highlight the last point of data in the sparkline group
## SparklineGroup.ShowLastPoint property
Indicates whether to highlight the last point of data in the sparkline group.
```csharp
public bool ShowLastPoint { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyShowLastPointDemo
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
// Configure sparkline appearance
CellsColor seriesColor = workbook.CreateCellsColor();
seriesColor.Color = Color.Orange;
group.SeriesColor = seriesColor;
group.LineWeight = 1.0;
// Enable and color the last point
group.ShowLastPoint = true;
CellsColor lastPointColor = workbook.CreateCellsColor();
lastPointColor.Color = Color.Yellow;
group.LastPointColor = lastPointColor;
// Save the workbook
workbook.Save("SparklineShowLastPointDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
