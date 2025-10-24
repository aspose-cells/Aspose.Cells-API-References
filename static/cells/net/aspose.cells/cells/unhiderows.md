##Cells.UnhideRows
Cells method. Unhides the hidden rows
## Cells.UnhideRows method
Unhides the hidden rows.
```csharp
public void UnhideRows(int row, int totalRows, double height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| totalRows | Int32 | The row number. |
| height | Double | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Hide rows 0-4
cells.HideRows(0, 5);
// Unhide rows 0-4 with height adjustment (-1 for auto-fit)
cells.UnhideRows(0, 5, -1);
// Verify rows are unhidden
for (int i = 0; i < 5; i++)
{
Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
