##Cells.GetGroupedRowOutlineLevel
Cells method. Gets the outline level zerobased of the row
## Cells.GetGroupedRowOutlineLevel method
Gets the outline level (zero-based) of the row.
```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | The row index. |
### Return Value
The outline level (zero-based) of the row.
### Remarks
If the row is not grouped, returns zero.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Group rows 0-3 (level 1)
cells.GroupRows(0, 3, false);
// Group rows 0-1 (level 2)
cells.GroupRows(0, 1, false);
// Get outline level for each row
for (int row = 0; row <= 4; row++)
{
int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
Console.WriteLine($"Row {row} outline level: {outlineLevel}");
}
// Ungroup all rows
cells.UngroupRows(0, 3);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
