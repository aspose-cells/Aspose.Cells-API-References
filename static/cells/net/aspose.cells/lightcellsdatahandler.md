##Interface LightCellsDataHandler
Aspose.Cells.LightCellsDataHandler interface. Represents cells data handler for reading large spreadsheet files in light weight mode
## LightCellsDataHandler interface
Represents cells data handler for reading large spreadsheet files in light weight mode.
```csharp
public interface LightCellsDataHandler
```
## Methods
| Name | Description |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Starts to process one cell. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Starts to process one row. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Prepares to process a cell. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Prepares to process a row. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Starts to process a worksheet. |
### Remarks
When reading a workbook by this mode, [`StartSheet`](./startsheet/) will be checked when reading every worksheet in the workbook. For one sheet, if [`StartSheet`](./startsheet/) gives true, then all data and properties of rows/cells of this sheet will be checked and processed by the implementation of this interface. For every row, [`StartRow`](./startrow/) will be called to check whether it need to be processed. If a row needs to be processed, properties of this row will be read firstly and user can access its properties by [`ProcessRow`](./processrow/). if row's cells need to be processed too, then [`ProcessRow`](./processrow/) should returns true and then [`StartCell`](./startcell/) will be called for every existing cell in this row to check whether one cell need to be processed. If one cell needs to be processed, then [`ProcessCell`](./processcell/) will be called to process the cell by the implementation of this interface.  Please note, user should only operate on the values and properties of current Row/Cell object provided by corresponding method. Because the cells data is read from the template file in streaming manner, most of other objects may be reset/update later after cells data has been loaded. So when user operating other objects in this implementation, those operations may be not able to affect the objects existing in the workbook. Or even worse, those operations may cause inconsistent data in the workbook and then cause unpected issue or exception later. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them after the workbook has been constructed.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataHandlerDemo : LightCellsDataHandler
{
public static void LightCellsDataHandlerExample()
{
// Create a workbook and load it with LightCellsDataHandler
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of LightCellsDataHandlerDemo
LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();
// Set the LightCellsDataHandler for the workbook
LoadOptions loadOptions = new LoadOptions();
loadOptions.LightCellsDataHandler = handler;
// Load the workbook with the specified load options
workbook = new Workbook("LargeFile_original.xlsx", loadOptions);
// Save the workbook to demonstrate the process
workbook.Save("ProcessedLargeFile.xlsx");
}
// Implement the StartSheet method
public bool StartSheet(Worksheet sheet)
{
Console.WriteLine("Starting to process sheet: " + sheet.Name);
return true; // Continue processing
}
// Implement the StartRow method
public bool StartRow(int rowIndex)
{
Console.WriteLine("Starting to process row: " + rowIndex);
return true; // Continue processing
}
// Implement the ProcessRow method
public bool ProcessRow(Row row)
{
Console.WriteLine("Processing row: " + row.Index);
return true; // Continue processing
}
// Implement the StartCell method
public bool StartCell(int columnIndex)
{
Console.WriteLine("Starting to process cell in column: " + columnIndex);
return true; // Continue processing
}
// Implement the ProcessCell method
public bool ProcessCell(Cell cell)
{
Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
return true; // Continue processing
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
