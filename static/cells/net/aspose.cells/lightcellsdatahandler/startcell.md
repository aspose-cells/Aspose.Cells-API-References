##LightCellsDataHandler.StartCell
LightCellsDataHandler method. Prepares to process a cell
## LightCellsDataHandler.StartCell method
Prepares to process a cell.
```csharp
public bool StartCell(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | column index of the cell to be processed |
### Return Value
whether this cell needs to be processed. false to ignore the cell and check the next one until reach the end of cells data of current row
### Remarks
It will be called when reaching an existing cell in current row. Current row is the row of last call of [`ProcessRow`](../processrow/).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class LightCellsDataHandlerMethodStartCellWithInt32Demo
{
public static void Run()
{
try
{
// Create a temporary input file
File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");
// Create load options with custom light cells handler
LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
var handler = new CustomLightCellsDataHandler();
loadOptions.LightCellsDataHandler = handler;
// Load workbook with custom handler
Workbook workbook = new Workbook("input.csv", loadOptions);
// Save the processed workbook
workbook.Save("output.xlsx");
Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing StartCell method: {ex.Message}");
}
}
private class CustomLightCellsDataHandler : LightCellsDataHandler
{
public bool StartSheet(Worksheet sheet)
{
return true; // Process all sheets
}
public bool StartRow(int rowIndex)
{
return true; // Process all rows
}
public bool StartCell(int columnIndex)
{
// Only process cells in column index 1 (second column)
return columnIndex == 1;
}
public bool ProcessCell(Cell cell)
{
// Double the value of cells in the second column
if (cell.IsNumericValue)
{
cell.PutValue(cell.DoubleValue * 2);
}
return true;
}
public bool ProcessRow(Row row)
{
return true; // Continue processing
}
}
}
}
```
### See Also
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
