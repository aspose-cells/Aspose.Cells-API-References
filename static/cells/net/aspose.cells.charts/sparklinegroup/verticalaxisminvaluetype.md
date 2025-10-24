##SparklineGroup.VerticalAxisMinValueType
SparklineGroup property. Represents the vertical axis minimum value type
## SparklineGroup.VerticalAxisMinValueType property
Represents the vertical axis minimum value type.
```csharp
public SparklineAxisMinMaxType VerticalAxisMinValueType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SparklineGroupPropertyVerticalAxisMinValueTypeDemo
{
public static void Run()
{
// Create a workbook and a worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["C1"].PutValue(1);
worksheet.Cells["D1"].PutValue(3);
// Define sparkline location
CellArea cellArea = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add sparkline group
int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
SparklineGroup group = worksheet.SparklineGroups[groupIndex];
group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);
// Set vertical axis min value type
group.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;
// Save the workbook
workbook.Save("SparklineVerticalAxisMinValueTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
