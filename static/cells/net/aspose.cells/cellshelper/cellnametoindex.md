##CellsHelper.CellNameToIndex
CellsHelper method. Gets the cell row and column indexes according to its name
## CellsHelper.CellNameToIndex method
Gets the cell row and column indexes according to its name.
```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Name of cell. |
| row | Int32& | Output row index |
| column | Int32& | Output column index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
{
public static void Run()
{
// Initialize variables to hold row and column indices
int rowIndex = -1;
int columnIndex = -1;
string cellName = "C5";
try
{
// Call CellNameToIndex method to convert cell name to row and column indices
CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);
// Display the results
Console.WriteLine($"Cell name: {cellName}");
Console.WriteLine($"Row index: {rowIndex}");
Console.WriteLine($"Column index: {columnIndex}");
// Create a workbook and demonstrate usage of the indices
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the cell using the obtained indices
Cell cell = worksheet.Cells[rowIndex, columnIndex];
cell.PutValue("Test Value");
// Save the workbook
workbook.Save("CellNameToIndexDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
}
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
