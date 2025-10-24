##Cells.HideRows
Cells method. Hides multiple rows
## Cells.HideRows method
Hides multiple rows.
```csharp
public void HideRows(int row, int totalRows)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| totalRows | Int32 | The row number. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodHideRowsWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
}
}
// Hide rows 3 to 5 (zero-based index: 2 to 4)
worksheet.Cells.HideRows(2, 3);
// Save the workbook
workbook.Save("HideRowsExample.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
