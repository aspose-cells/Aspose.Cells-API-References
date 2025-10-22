##Enum SparklineAxisMinMaxType
Aspose.Cells.Charts.SparklineAxisMinMaxType enum. Represents the minimum and maximum value types for the sparkline vertical axis
## SparklineAxisMinMaxType enumeration
Represents the minimum and maximum value types for the sparkline vertical axis.
```csharp
public enum SparklineAxisMinMaxType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| AutoIndividual | `0` | Automatic for each sparkline. |
| Group | `1` | Same for all sparklines in the group. |
| Custom | `2` | Custom value for sparkline. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class SparklineAxisMinMaxTypeDemo
{
public static void SparklineAxisMinMaxTypeExample()
{
// Create a workbook and a worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["C1"].PutValue(1);
worksheet.Cells["D1"].PutValue(3);
// Define the CellArea
CellArea cellArea = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add a sparkline group to the worksheet
int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);
// Set properties for the sparkline group
sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;
// Create CellsColor
CellsColor highPointColor = workbook.CreateCellsColor();
highPointColor.Color = Color.Green;
sparklineGroup.HighPointColor = highPointColor;
CellsColor lowPointColor = workbook.CreateCellsColor();
lowPointColor.Color = Color.Red;
sparklineGroup.LowPointColor = lowPointColor;
// Set additional properties
sparklineGroup.ShowHighPoint = true;
sparklineGroup.ShowLowPoint = true;
sparklineGroup.LineWeight = 1.0;
// Save the workbook
workbook.Save("SparklineAxisMinMaxTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
