##SparklineGroup.NegativePointsColor
SparklineGroup property. Gets and sets the color of the negative values on the sparkline group
## SparklineGroup.NegativePointsColor property
Gets and sets the color of the negative values on the sparkline group.
```csharp
public CellsColor NegativePointsColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyNegativePointsColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add data with negative values to demonstrate negative points
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(-2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(-3);
// Define the CellArea for the sparkline
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
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Configure negative points color
group.ShowNegativePoints = true;
CellsColor negativePointsColor = workbook.CreateCellsColor();
negativePointsColor.Color = Color.Blue;
group.NegativePointsColor = negativePointsColor;
workbook.Save("SparklineNegativePointsColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
