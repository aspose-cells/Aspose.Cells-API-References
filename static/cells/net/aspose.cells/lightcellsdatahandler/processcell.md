##LightCellsDataHandler.ProcessCell
LightCellsDataHandler method. Starts to process one cell
## LightCellsDataHandler.ProcessCell method
Starts to process one cell.
```csharp
public bool ProcessCell(Cell cell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Cell object which is being processed currently |
### Return Value
whether this cell needs to be kept in cells model of current sheet. Commonly it should be false so that all cells will not be kept in memory after being processed and then memory be saved. For some special purpose such as user needs to access some cells later after the whole workbook having been processed, user can make this method return true to keep those special cells in Cells model and access them later by APIs such as Cells[row, column]. However, keeping cells data in Cells model will requires more memory and if all cells are kept then reading template file in LightCells mode will become same with reading it in normal way.
### Remarks
It will be called after one cell's data has been read.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class LightCellsDataHandlerMethodProcessCellWithCellDemo
{
public static void Run()
{
try
{
// Create temporary data file
File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");
// Create load options with custom light cells handler
LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
var handler = new CustomLightCellsDataHandler();
loadOptions.LightCellsDataHandler = handler;
// Load workbook with custom handler
Workbook workbook = new Workbook("input.txt", loadOptions);
// Save processed results
workbook.Save("output.xlsx");
Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
return true; // Process all cells
}
public bool ProcessCell(Cell cell)
{
// Double numeric values and mark strings
if (cell.IsNumericValue)
{
cell.PutValue(cell.DoubleValue * 2);
}
else if (cell.Type == CellValueType.IsString)
{
cell.PutValue($"TEXT: {cell.StringValue}");
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
* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
