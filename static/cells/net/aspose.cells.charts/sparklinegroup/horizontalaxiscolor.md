##SparklineGroup.HorizontalAxisColor
SparklineGroup property. Gets and sets the color of the horizontal axis in the sparkline group
## SparklineGroup.HorizontalAxisColor property
Gets and sets the color of the horizontal axis in the sparkline group.
```csharp
public CellsColor HorizontalAxisColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyHorizontalAxisColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(5);
sheet.Cells["A2"].PutValue(3);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["A4"].PutValue(4);
// Create sparkline group
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 3;
ca.StartColumn = 4;
ca.EndColumn = 4;
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Set horizontal axis color
CellsColor axisColor = workbook.CreateCellsColor();
axisColor.Color = Color.Blue;
group.HorizontalAxisColor = axisColor;
group.ShowHorizontalAxis = true;
// Save the workbook
workbook.Save("SparklineHorizontalAxisColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
