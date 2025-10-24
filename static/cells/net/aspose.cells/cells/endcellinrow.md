##Cells.EndCellInRow
Cells method. Gets the last cell in this row
## EndCellInRow(int) {#endcellinrow}
Gets the last cell in this row.
```csharp
public Cell EndCellInRow(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
### Return Value
Cell object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodEndCellInRowWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data in row 5 (0-based index)
worksheet.Cells[5, 2].PutValue("Data1");
worksheet.Cells[5, 4].PutValue("Data2");
worksheet.Cells[5, 6].PutValue("Data3");
try
{
// Call EndCellInRow with row index 5
Cell endCell = worksheet.Cells.EndCellInRow(5);
if (endCell != null)
{
Console.WriteLine($"Last cell in row 5: {endCell.Name}");
Console.WriteLine($"Cell value: {endCell.StringValue}");
}
else
{
Console.WriteLine("No cells found in row 5");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing EndCellInRow: {ex.Message}");
}
// Save the workbook
workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## EndCellInRow(int, int, int, int) {#endcellinrow_1}
Gets the last cell with maximum row index in this range.
```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |
### Return Value
Cell object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data in the worksheet
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
}
}
// Get the end cell in row 3 between columns 1 to 4
Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);
// Output the end cell's row and column indices
Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
