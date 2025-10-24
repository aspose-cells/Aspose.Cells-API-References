##Cells.CheckCell
Cells method. Gets the Cell element or null at the specified cell row index and column index
## Cells.CheckCell method
Gets the [`Cell`](../../cell/) element or null at the specified cell row index and column index.
```csharp
public Cell CheckCell(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
| column | Int32 | Column index |
### Return Value
Return Cell object if a Cell object exists. Return null if the cell does not exist.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCheckCellWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set values in cells
cells[0, 0].PutValue("Hello");
cells[1, 1].PutValue(123);
cells[2, 2].PutValue(DateTime.Now);
// Check cells using CheckCell method with Int32 parameters
Cell cell1 = cells.CheckCell(0, 0);
Console.WriteLine("Cell A1 value: " + cell1.StringValue);
Cell cell2 = cells.CheckCell(1, 1);
Console.WriteLine("Cell B2 value: " + cell2.StringValue);
Cell cell3 = cells.CheckCell(2, 2);
Console.WriteLine("Cell C3 value: " + cell3.StringValue);
// Check non-existent cell (will return null)
Cell cell4 = cells.CheckCell(10, 10);
if (cell4 == null)
{
Console.WriteLine("Cell K11 doesn't exist (as expected)");
}
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
