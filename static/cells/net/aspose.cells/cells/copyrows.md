##Cells.CopyRows
Cells method. Copies data and formats of some whole rows
## CopyRows(Cells, int, int, int) {#copyrows}
Copies data and formats of some whole rows.
```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook destinationWorkbook = new Workbook();
Workbook sourceWorkbook = new Workbook();
// Add some sample data to the source workbook
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
sourceSheet.Cells["A1"].PutValue("Source Data 1");
sourceSheet.Cells["A2"].PutValue("Source Data 2");
sourceSheet.Cells["A3"].PutValue("Source Data 3");
// Get the cells from both workbooks
Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
Cells sourceCells = sourceSheet.Cells;
// Copy all rows from source to destination starting at row 0 in destination
destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);
// Save the result
destinationWorkbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}
Copies data and formats of some whole rows.
```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex,
int rowNumber, CopyOptions copyOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data and hyperlinks
worksheet.Cells["A1"].PutValue("Source Data");
worksheet.Cells["A4"].PutValue("Row 4 Data");
worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");
// Insert a blank row at row 5
worksheet.Cells.InsertRows(5, 1);
// Copy row 4 to row 5 without CopyOptions
worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);
// Reset the worksheet
worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
worksheet.Hyperlinks.Clear();
worksheet.Cells["A4"].PutValue("Row 4 Data");
worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");
// Insert a blank row at row 5 again
worksheet.Cells.InsertRows(5, 1);
// Copy row 4 to row 5 with CopyOptions
CopyOptions options = new CopyOptions();
options.ExtendToAdjacentRange = true;
worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
}
}
}
```
### See Also
* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}
Copies data and formats of some whole rows.
```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex,
int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
Worksheet sourceSheet = workbook.Worksheets[0];
Worksheet destinationSheet = workbook.Worksheets.Add("DestinationSheet");
// Populate source worksheet with sample data
sourceSheet.Cells["A1"].PutValue("Source Row 1");
sourceSheet.Cells["A2"].PutValue("Source Row 2");
sourceSheet.Cells["A3"].PutValue("Source Row 3");
try
{
// Create copy and paste options
CopyOptions copyOptions = new CopyOptions();
PasteOptions pasteOptions = new PasteOptions();
// Copy 3 rows from source sheet starting at row 0 to destination sheet starting at row 5
destinationSheet.Cells.CopyRows(
sourceSheet.Cells, // Source cells
0,                  // Source row index
5,                  // Destination row index
3,                  // Number of rows to copy
copyOptions,
pasteOptions
);
Console.WriteLine("Rows copied successfully from row 0-2 to row 5-7 in destination sheet");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing CopyRows method: {ex.Message}");
}
// Save the result
workbook.Save("CellsMethodCopyRowsWithOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
