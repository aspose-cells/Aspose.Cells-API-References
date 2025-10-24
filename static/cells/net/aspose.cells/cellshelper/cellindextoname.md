##CellsHelper.CellIndexToName
CellsHelper method. Gets cell name according to its row and column indexes
## CellsHelper.CellIndexToName method
Gets cell name according to its row and column indexes.
```csharp
public static string CellIndexToName(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |
### Return Value
Name of cell.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Data");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["C3"].PutValue(20);
// Get the cell name from row and column indices
string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)
// Output the result
Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
