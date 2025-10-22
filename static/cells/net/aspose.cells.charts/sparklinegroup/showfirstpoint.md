##SparklineGroup.ShowFirstPoint
SparklineGroup property. Indicates whether to highlight the first point of data in the sparkline group
## SparklineGroup.ShowFirstPoint property
Indicates whether to highlight the first point of data in the sparkline group.
```csharp
public bool ShowFirstPoint { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyShowFirstPointDemo
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
// Define sparkline location
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add sparkline group
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Configure sparkline appearance
group.ShowFirstPoint = true;
CellsColor firstPointColor = workbook.CreateCellsColor();
firstPointColor.Color = Color.Purple;
group.FirstPointColor = firstPointColor;
// Save the workbook
workbook.Save("SparklineShowFirstPointDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
