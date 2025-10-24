##Cells.DeleteRange
Cells method. Deletes a range of cells and shift cells according to the shift option
## Cells.DeleteRange method
Deletes a range of cells and shift cells according to the shift option.
```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn,
ShiftType shiftType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |
| shiftType | ShiftType | Shift cells option. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Populate some sample data
sheet.Cells["A1"].PutValue("A1");
sheet.Cells["B1"].PutValue("B1");
sheet.Cells["C1"].PutValue("C1");
sheet.Cells["A2"].PutValue("A2");
sheet.Cells["B2"].PutValue("B2");
sheet.Cells["C2"].PutValue("C2");
// Delete range and shift left
sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);
// Save the workbook
workbook.Save("DeleteRangeExample.xlsx");
}
}
}
```
### See Also
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
