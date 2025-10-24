##SparklineGroup.LineWeight
SparklineGroup property. Gets and sets the line weight in each line sparkline in the sparkline group in the unit of points
## SparklineGroup.LineWeight property
Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.
```csharp
public double LineWeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyLineWeightDemo
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
// Set LineWeight property
group.LineWeight = 2.5; // Thicker line weight for visibility
workbook.Save("SparklineLineWeightDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
