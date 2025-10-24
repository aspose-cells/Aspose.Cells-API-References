##Cells.CopyColumns
Cells method. Copies data and formats of a whole column
## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}
Copies data and formats of a whole column.
```csharp
public void CopyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex,
int columnNumber, PasteOptions pasteOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |
| columnNumber | Int32 | The copied column number. |
| pasteOptions | PasteOptions | the options of pasting. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCopyColumnsWithCellsInt32Int32Int32PasteOptioDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
// Create another workbook as destination
Workbook destWorkbook = new Workbook();
Worksheet destWorksheet = destWorkbook.Worksheets[0];
// Copy columns with formatting only
try
{
destWorksheet.Cells.CopyColumns(
worksheet.Cells,
0, // source column index
0, // destination column index
2, // column count (copy 2 columns)
new PasteOptions() { PasteType = PasteType.Formats });
Console.WriteLine("Columns copied successfully with formatting only.");
}
catch (Exception ex)
{
Console.WriteLine("Error copying columns: " + ex.Message);
}
// Save the workbook
workbook.Save("CopyColumnsDemo.xlsx");
}
}
}
```
### See Also
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CopyColumns(Cells, int, int, int) {#copycolumns}
Copies data and formats of a whole column.
```csharp
public void CopyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex,
int columnNumber)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |
| columnNumber | Int32 | The copied column number. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet worksheet = wb.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data to columns
cells["A1"].PutValue("Source1");
cells["B1"].PutValue("Source2");
cells["C1"].PutValue("Source3");
cells["D1"].PutValue("Source4");
cells["E1"].PutValue("Source5");
// Copy columns from column index 1 (B) to column index 3 (D), copy 1 column
cells.CopyColumns(cells, 1, 3, 1);
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}
Copies data and formats of the whole columns.
```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns,
int destinationColumnIndex, int destinationTotalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| sourceTotalColumns | Int32 | The number of the source columns. |
| destinationColumnIndex | Int32 | Destination column index. |
| destinationTotalColumns | Int32 | The number of the destination columns. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate source columns (columns 0 and 1)
cells[0, 0].Value = "Header 1";
cells[0, 1].Value = "Header 2";
for (int row = 1; row <= 4; row++)
{
cells[row, 0].Value = row * 100;
cells[row, 1].Value = row * 200;
}
try
{
// Copy 2 columns from index 0 to destination index 3, inserting 2 columns
cells.CopyColumns(cells, 0, 2, 3, 2);
Console.WriteLine("Copied 2 source columns to destination position successfully");
// Verify copy by checking destination columns (3 and 4)
Console.WriteLine($"Destination column 3 value: {cells[0, 3].StringValue}");
Console.WriteLine($"Destination column 4 value: {cells[0, 4].StringValue}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing CopyColumns: {ex.Message}");
}
// Save the modified workbook
workbook.Save("CellsMethodCopyColumnsWithCellsInt32Int32Int32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
