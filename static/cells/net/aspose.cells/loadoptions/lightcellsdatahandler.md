##LoadOptions.LightCellsDataHandler
LoadOptions property. The data handler for processing cells data when reading template file
## LoadOptions.LightCellsDataHandler property
The data handler for processing cells data when reading template file.
```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyLightCellsDataHandlerDemo
{
public static void Run()
{
// Create a custom LightCellsDataHandler to process cells data
var dataHandler = new CustomLightCellsDataHandler();
// Create load options and set the data handler
LoadOptions loadOptions = new LoadOptions();
loadOptions.LightCellsDataHandler = dataHandler;
// Load workbook with the custom handler
using (Workbook workbook = new Workbook("sample.xlsx", loadOptions))
{
Console.WriteLine("Workbook processed successfully with LightCellsDataHandler");
}
}
}
public class CustomLightCellsDataHandler : LightCellsDataHandler
{
public bool StartSheet(Worksheet sheet)
{
Console.WriteLine($"Processing sheet: {sheet.Name}");
return true; // Continue processing this sheet
}
public bool StartRow(int rowIndex)
{
Console.WriteLine($"  Starting row: {rowIndex}");
return true; // Continue processing this row
}
public bool ProcessRow(Row row)
{
// You can process row data here if needed
return true;
}
public bool StartCell(int columnIndex)
{
Console.WriteLine($"    Starting cell at column: {columnIndex}");
return true; // Continue processing this cell
}
public bool ProcessCell(Cell cell)
{
Console.WriteLine($"      Cell[{cell.Row},{cell.Column}]: {cell.Value}");
return true;
}
}
}
```
### See Also
* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
