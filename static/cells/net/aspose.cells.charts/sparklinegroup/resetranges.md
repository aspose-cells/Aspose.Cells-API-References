##SparklineGroup.ResetRanges
SparklineGroup method. Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges
## SparklineGroup.ResetRanges method
Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.
```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline group. |
| isVertical | Boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some data to the worksheet
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
// Define the CellArea for the sparkline
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add a sparkline group to the worksheet
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Prepare parameters for ResetRanges
string dataRange = "A1:D1";
bool isVertical = false;
CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);
try
{
// Call ResetRanges with parameters (String, Boolean, CellArea)
group.ResetRanges(dataRange, isVertical, locationRange);
Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
}
// Save the result
workbook.Save("SparklineGroupResetRangesDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
