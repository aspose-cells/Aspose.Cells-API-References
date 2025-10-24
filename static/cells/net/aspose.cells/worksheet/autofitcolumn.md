##Worksheet.AutoFitColumn
Worksheet method. Autofits the column width
## AutoFitColumn(int, int, int) {#autofitcolumn_1}
Autofits the column width.
```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| firstRow | Int32 | First row index. |
| lastRow | Int32 | Last row index. |
### Remarks
This method autofits a row based on content in a range of cells within the row.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with sample data that will require column width adjustment
worksheet.Cells["A1"].PutValue("Short text");
worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
try
{
Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
// Call AutoFitColumn on column A (index 0) for rows 0 to 2 (zero-based)
worksheet.AutoFitColumn(0, 0, 2);
Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
// Display the effect by showing the column width before and after
Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
}
// Save the result
workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitColumn(int) {#autofitcolumn}
Autofits the column width.
```csharp
public void AutoFitColumn(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
### Remarks
AutoFitColumn is an imprecise function.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitColumnWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells in column 4 (0-based index)
worksheet.Cells["D1"].PutValue("This is a test");
worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
// Auto-fit column 4 (0-based index)
worksheet.AutoFitColumn(3);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
