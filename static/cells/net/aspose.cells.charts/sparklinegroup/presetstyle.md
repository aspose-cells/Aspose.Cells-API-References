##SparklineGroup.PresetStyle
SparklineGroup property. Gets and sets the preset style type of the sparkline group
## SparklineGroup.PresetStyle property
Gets and sets the preset style type of the sparkline group.
```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyPresetStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(3);
worksheet.Cells["C1"].PutValue(7);
worksheet.Cells["D1"].PutValue(2);
worksheet.Cells["E1"].PutValue(9);
// Create sparkline group
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 5;
ca.EndColumn = 5;
int index = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:E1", false, ca);
SparklineGroup group = worksheet.SparklineGroups[index];
// Apply preset style
group.PresetStyle = SparklinePresetStyleType.Style5;
workbook.Save("SparklinePresetStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
