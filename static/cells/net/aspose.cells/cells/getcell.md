##Cells.GetCell
Cells method. Gets the Cell element or null at the specified cell row index and column index
## Cells.GetCell method
Gets the [`Cell`](../../cell/) element or null at the specified cell row index and column index.
```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
| column | Int32 | Column index |
### Return Value
Return Cell object if a Cell object exists. Return null if the cell does not exist.
### Remarks
NOTE: This member is now obsolete. Instead, please use CheckCell(int row, int column) method. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetCellWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell at row 1, column 2 (0-based index)
Cell cell = worksheet.Cells.GetCell(1, 2);
// Set value and style for demonstration
cell.PutValue("Test Value");
Style style = cell.GetStyle();
style.Font.IsBold = true;
cell.SetStyle(style);
// Save the workbook
workbook.Save("GetCellDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
