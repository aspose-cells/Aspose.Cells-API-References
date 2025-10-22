##SparklineGroup.ShowNegativePoints
SparklineGroup property. Indicates whether to highlight the negative values on the sparkline group with a different color or marker
## SparklineGroup.ShowNegativePoints property
Indicates whether to highlight the negative values on the sparkline group with a different color or marker.
```csharp
public bool ShowNegativePoints { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyShowNegativePointsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add data with negative values to demonstrate ShowNegativePoints
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
// Add a sparkline group
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Configure sparkline group properties
group.ShowNegativePoints = true;
CellsColor negativePointsColor = workbook.CreateCellsColor();
negativePointsColor.Color = Color.Blue;
group.NegativePointsColor = negativePointsColor;
// Save the workbook
workbook.Save("SparklineNegativePointsDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
