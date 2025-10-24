##Cells.UnhideRow
Cells method. Unhides a row
## Cells.UnhideRow method
Unhides a row.
```csharp
public void UnhideRow(int row, double height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| height | Double | Row height. The row's height will be changed only when the row is hidden and given height value is positive. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodUnhideRowWithInt32DoubleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Hide row 5
worksheet.Cells.HideRow(5);
// Unhide row 5 with a height of 12.75
worksheet.Cells.UnhideRow(5, 12.75);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
