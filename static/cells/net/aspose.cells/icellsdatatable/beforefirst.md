##ICellsDataTable.BeforeFirst
ICellsDataTable method. Move the cursor to the front of this object just before the first row
## ICellsDataTable.BeforeFirst method
Move the cursor to the front of this object, just before the first row.
```csharp
public void BeforeFirst()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class ICellsDataTableMethodBeforeFirstDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
DataTable sourceTable = new DataTable("Employees");
sourceTable.Columns.Add("Name", typeof(string));
sourceTable.Columns.Add("Department", typeof(string));
sourceTable.Rows.Add("John Doe", "Engineering");
sourceTable.Rows.Add("Jane Smith", "Marketing");
// Import data to worksheet
ImportTableOptions importOptions = new ImportTableOptions();
importOptions.IsFieldNameShown = true;
worksheet.Cells.ImportData(sourceTable, 0, 0, importOptions);
// Get ICellsDataTable by exporting the data from the worksheet
ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, sourceTable.Rows.Count + 1, sourceTable.Columns.Count);
try
{
// Reset cursor to beginning of data table
dataTable.BeforeFirst();
Console.WriteLine("Reading data from ICellsDataTable:");
while (dataTable.Next())
{
Console.WriteLine(
$"Name: {dataTable[0]}, " +
$"Department: {dataTable[1]}");
}
// Demonstrate cursor reset
dataTable.BeforeFirst();
Console.WriteLine("\nCursor reset. Reading data again:");
while (dataTable.Next())
{
Console.WriteLine(
$"Name: {dataTable["Name"]}, " +
$"Department: {dataTable["Department"]}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing BeforeFirst method: {ex.Message}");
}
workbook.Save("ICellsDataTableBeforeFirstDemo.xlsx");
}
}
}
```
### See Also
* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
