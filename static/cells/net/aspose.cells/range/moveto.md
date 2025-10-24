##Range.MoveTo
Range method. Move the current range to the dest range
## Range.MoveTo method
Move the current range to the dest range.
```csharp
public void MoveTo(int destRow, int destColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| destRow | Int32 | The start row of the dest range. |
| destColumn | Int32 | The start column of the dest range. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodMoveToWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a sample range (A1:B2)
Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
// Put some data in the range for demonstration
originalRange[0, 0].PutValue("A1");
originalRange[0, 1].PutValue("B1");
originalRange[1, 0].PutValue("A2");
originalRange[1, 1].PutValue("B2");
// Move the range down by 1 row (to A2:B3)
originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
