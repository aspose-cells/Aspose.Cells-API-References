##SparklineGroup.ShowHighPoint
SparklineGroup property. Indicates whether to highlight the highest points of data in the sparkline group
## SparklineGroup.ShowHighPoint property
Indicates whether to highlight the highest points of data in the sparkline group.
```csharp
public bool ShowHighPoint { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyShowHighPointDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["C1"].PutValue(1);
worksheet.Cells["D1"].PutValue(3);
// Create sparkline group
CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };
int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
SparklineGroup group = worksheet.SparklineGroups[groupIndex];
// Add sparkline
group.Sparklines.Add("A1:D1", 0, 4);
// Configure high point display
group.ShowHighPoint = true;
CellsColor highColor = workbook.CreateCellsColor();
highColor.Color = System.Drawing.Color.Green;
group.HighPointColor = highColor;
// Save workbook
workbook.Save("SparklineHighPointDemo.xlsx");
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
