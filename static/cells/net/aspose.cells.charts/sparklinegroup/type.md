##SparklineGroup.Type
SparklineGroup property. Indicates the sparkline type of the sparkline group
## SparklineGroup.Type property
Indicates the sparkline type of the sparkline group.
```csharp
public SparklineType Type { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyTypeDemo
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
// Create sparkline group with Column type
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 4;
ca.EndColumn = 4;
int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Change the sparkline type to Line
group.Type = SparklineType.Line;
// Add sparkline to the group
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Save the workbook
workbook.Save("SparklineTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
