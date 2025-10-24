##Cells.IsDeletingRangeEnabled
Cells method. Check whether the range could be deleted
## Cells.IsDeletingRangeEnabled method
Check whether the range could be deleted.
```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row index of the range. |
| startColumn | Int32 | The start column index of the range. |
| totalRows | Int32 | The number of the rows in the range. |
| totalColumns | Int32 | The number of the columns in the range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodIsDeletingRangeEnabledWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate sample data in cells A1:C5
for (int row = 0; row < 5; row++)
{
for (int col = 0; col < 3; col++)
{
cells[row, col].Value = $"Data{row}_{col}";
}
}
try
{
// Check if deleting 5 rows x 3 columns starting from A1 is enabled
bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
Console.WriteLine($"Can delete range: {canDelete}");
if (canDelete)
{
// Delete the range A1:C5 and shift cells up
cells.DeleteRange(0, 0, 4, 2, ShiftType.Up);
Console.WriteLine("Deleted range A1:C5 successfully");
}
workbook.Save("IsDeletingRangeEnabledOutput.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error during range deletion: {ex.Message}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
