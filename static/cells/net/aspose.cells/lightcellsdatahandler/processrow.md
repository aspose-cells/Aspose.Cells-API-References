##LightCellsDataHandler.ProcessRow
LightCellsDataHandler method. Starts to process one row
## LightCellsDataHandler.ProcessRow method
Starts to process one row.
```csharp
public bool ProcessRow(Row row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | Row object which is being processed currently. |
### Return Value
whether this row's cells need to be processed. false to ignore all cells in this row.
### Remarks
It will be called after row's properties such as height, style, ...etc. have been read. However, cells in this row has not been read yet.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataHandlerMethodProcessRowWithRowDemo
{
public static void Run()
{
try
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].Value = "Test Data";
worksheet.Cells["A2"].Value = 100;
worksheet.Cells["B2"].Value = 200;
// Create custom handler
var handler = new CustomRowHandler();
// Process the first row
Row firstRow = worksheet.Cells.Rows[0];
bool result = handler.ProcessRow(firstRow);
Console.WriteLine($"ProcessRow returned: {result}");
Console.WriteLine($"Row height after processing: {firstRow.Height}");
workbook.Save("ProcessRowDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
}
}
private class CustomRowHandler : LightCellsDataHandler
{
public bool ProcessRow(Row row)
{
// Demonstrate accessing row properties
Console.WriteLine($"Processing row index: {row.Index}");
Console.WriteLine($"Row is hidden: {row.IsHidden}");
Console.WriteLine($"Row is blank: {row.IsBlank}");
// Modify row height if it's not the header row
if (row.Index > 0)
{
row.Height = 25.0;
}
return true;
}
public bool StartSheet(Worksheet sheet) => true;
public bool StartRow(int rowIndex) => true;
public bool StartCell(int columnIndex) => true;
public bool ProcessCell(Cell cell) => true;
}
}
}
```
### See Also
* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
