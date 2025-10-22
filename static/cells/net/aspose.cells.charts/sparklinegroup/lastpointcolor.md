##SparklineGroup.LastPointColor
SparklineGroup property. Gets and sets the color of the last point of data in the sparkline group
## SparklineGroup.LastPointColor property
Gets and sets the color of the last point of data in the sparkline group.
```csharp
public CellsColor LastPointColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyLastPointColorDemo
{
public static void Run()
{
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
// Configure sparkline appearance
group.ShowLastPoint = true;
CellsColor lastPointColor = workbook.CreateCellsColor();
lastPointColor.Color = Color.Yellow;
group.LastPointColor = lastPointColor;
// Save the workbook
workbook.Save("SparklineLastPointColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
