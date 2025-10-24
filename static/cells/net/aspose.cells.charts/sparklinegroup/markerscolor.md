##SparklineGroup.MarkersColor
SparklineGroup property. Gets and sets the color of points in each line sparkline in the sparkline group
## SparklineGroup.MarkersColor property
Gets and sets the color of points in each line sparkline in the sparkline group.
```csharp
public CellsColor MarkersColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyMarkersColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Sample data
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
group.ShowMarkers = true;
CellsColor markersColor = workbook.CreateCellsColor();
markersColor.Color = Color.Black;
group.MarkersColor = markersColor;
// Save the workbook
workbook.Save("SparklineMarkersColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
