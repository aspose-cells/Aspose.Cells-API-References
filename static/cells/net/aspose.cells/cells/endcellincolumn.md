##Cells.EndCellInColumn
Cells method. Gets the last cell in this column
## EndCellInColumn(int) {#endcellincolumn}
Gets the last cell in this column.
```csharp
public Cell EndCellInColumn(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
### Return Value
Cell object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodEndCellInColumnWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
worksheet.Cells["A4"].PutValue("Data3");
worksheet.Cells["B1"].PutValue("Value1");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Get the last cell in column A (column index 0)
Cell lastCell = worksheet.Cells.EndCellInColumn(0);
Console.WriteLine("Last cell in column A: Row " + lastCell.Row + ", Value: " + lastCell.StringValue);
// Iterate through all rows in column A
for (int row = 0; row <= lastCell.Row; row++)
{
Cell cell = worksheet.Cells[row, 0];
Console.WriteLine("Row " + row + ": " + cell.StringValue);
}
// Save the workbook
workbook.Save("EndCellInColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}
Gets the last cell with maximum column index in this range.
```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
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
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data in column B (index 1)
worksheet.Cells[0, 1].PutValue("Data 1");
worksheet.Cells[2, 1].PutValue("Data 2");
worksheet.Cells[3, 1].PutValue("Data 3");
try
{
// Call EndCellInColumn with parameters: startRow=0, endRow=5, startColumn=1, endColumn=1
Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);
if (result != null)
{
Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
// Mark the found cell
result.PutValue("Last Cell");
Style style = result.GetStyle();
style.Font.IsBold = true;
result.SetStyle(style);
}
else
{
Console.WriteLine("No cells found in specified range");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing EndCellInColumn method: {ex.Message}");
}
// Save the workbook
workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
