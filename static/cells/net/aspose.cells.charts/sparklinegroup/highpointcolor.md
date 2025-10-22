##SparklineGroup.HighPointColor
SparklineGroup property. Gets and sets the color of the highest points of data in the sparkline group
## SparklineGroup.HighPointColor property
Gets and sets the color of the highest points of data in the sparkline group.
```csharp
public CellsColor HighPointColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyHighPointColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
group.ShowHighPoint = true;
group.HighPointColor.Color = Color.Green;
workbook.Save("SparklineHighPointColorDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
