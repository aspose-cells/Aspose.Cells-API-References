##Cells.DeleteRows
Cells method. Deletes multiple rows
## DeleteRows(int, int) {#deleterows}
Deletes multiple rows.
```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | The first row index to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
### Remarks
If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteRowsWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate some sample data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
}
}
Console.WriteLine("Before deleting rows:");
PrintCellValues(cells, 0, 9, 0, 4);
// Delete 2 rows starting from row index 2 (3rd row)
cells.DeleteRows(2, 2);
Console.WriteLine("\nAfter deleting rows 3-4:");
PrintCellValues(cells, 0, 7, 0, 4);
// Save the workbook
workbook.Save("output.xlsx");
}
private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
{
for (int i = startRow; i <= endRow; i++)
{
for (int j = startCol; j <= endCol; j++)
{
Console.Write($"{cells[i, j].StringValue}\t");
}
Console.WriteLine();
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DeleteRows(int, int, bool) {#deleterows_2}
Deletes multiple rows in the worksheet.
```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the first row to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Import data into cells
worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);
// Create a table
ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
table.ShowHeaderRow = false;
Console.WriteLine("Before DeleteRows:");
Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
Console.WriteLine($"Table Start Row: {table.StartRow}");
Console.WriteLine($"Table End Row: {table.EndRow}");
// Delete row at index 1 (second row) with update reference
worksheet.Cells.DeleteRows(1, 1, true);
Console.WriteLine("\nAfter DeleteRows:");
Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
Console.WriteLine($"Table Start Row: {table.StartRow}");
Console.WriteLine($"Table End Row: {table.EndRow}");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DeleteRows(int, int, DeleteOptions) {#deleterows_1}
Deletes multiple rows in the worksheet.
```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the first row to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
| options | DeleteOptions | Options for the deleting operation |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Set sample data and formulas
cells["A1"].PutValue(10);
cells["A2"].PutValue(20);
cells["A3"].PutValue(30);
cells["B1"].Formula = "=SUM(A1:A3)";
// Delete row 2 without monitoring (since FormulaChangeMonitor is not available)
cells.DeleteRows(1, 1, new DeleteOptions());
Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
}
}
}
```
### See Also
* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
