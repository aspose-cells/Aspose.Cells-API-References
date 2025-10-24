##SparklineGroupCollection.ClearSparklineGroups
SparklineGroupCollection method. Clears the sparkline groups that overlaps an area of cells
## SparklineGroupCollection.ClearSparklineGroups method
Clears the sparkline groups that overlaps an area of cells.
```csharp
public void ClearSparklineGroups(CellArea cellArea)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Specifies the area of cells |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
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
try
{
// Call the ClearSparklineGroups method with CellArea parameter
sheet.SparklineGroups.ClearSparklineGroups(ca);
Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
// Verify the sparkline groups count after clearing
Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
}
// Save the result
workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
