##SparklineGroup.LowPointColor
SparklineGroup property. Gets and sets the color of the lowest points of data in the sparkline group
## SparklineGroup.LowPointColor property
Gets and sets the color of the lowest points of data in the sparkline group.
```csharp
public CellsColor LowPointColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyLowPointColorDemo
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
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add sparkline group using correct API
int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = worksheet.SparklineGroups[idx];
group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);
// Customize sparkline appearance
group.ShowLowPoint = true;
group.LowPointColor.Color = Color.Red;
workbook.Save("SparklineLowPointColorDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
