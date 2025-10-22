##ImportTableOptions.ShiftFirstRowDown
ImportTableOptions property. Indicates whether shifting the first row down when inserting rows
## ImportTableOptions.ShiftFirstRowDown property
Indicates whether shifting the first row down when inserting rows.
```csharp
public bool ShiftFirstRowDown { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyShiftFirstRowDownDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create sample DataTable
DataTable table = new DataTable();
table.Columns.Add("Column1");
table.Columns.Add("Column2");
table.Rows.Add("Header1", "Header2");
table.Rows.Add("Data1", "Data2");
table.Rows.Add("Data3", "Data4");
// Import with ShiftFirstRowDown = false (default behavior)
var options1 = new ImportTableOptions
{
IsFieldNameShown = false,
ShiftFirstRowDown = false
};
cells.ImportData(table, 0, 0, options1);
Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);
// Clear worksheet and import with ShiftFirstRowDown = true
workbook.Worksheets[0].Cells.Clear();
var options2 = new ImportTableOptions
{
IsFieldNameShown = false,
ShiftFirstRowDown = true
};
cells.ImportData(table, 0, 0, options2);
Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);
// Save the workbook
workbook.Save("ShiftFirstRowDownDemo.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
