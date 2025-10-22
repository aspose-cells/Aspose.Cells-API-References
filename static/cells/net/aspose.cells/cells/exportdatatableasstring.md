##Cells.ExportDataTableAsString
Cells method. Exports data in the Cells collection to a DataTable object
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}
Exports data in the [`Cells`](../) collection to a DataTable object.
```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows,
int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
### Return Value
Exported DataTable object.
### Remarks
All data in the [`Cells`](../) collection are converted to strings.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data to cells
cells["A1"].PutValue("Column1");
cells["B1"].PutValue("Column2");
cells["A2"].PutValue("Value1");
cells["B2"].PutValue("Value2");
// Export data to DataTable as strings
DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);
// Display the exported data
Console.WriteLine("Exported DataTable:");
foreach (DataColumn column in dataTable.Columns)
{
Console.Write(column.ColumnName + "\t");
}
Console.WriteLine();
foreach (DataRow row in dataTable.Rows)
{
foreach (var item in row.ItemArray)
{
Console.Write(item.ToString() + "\t");
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
## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}
Exports data in the [`Cells`](../) collection to a DataTable object.
```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows,
int totalColumns, bool exportColumnName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| exportColumnName | Boolean | Indicates whether the data in the first row are exported to the column name of the DataTable. |
### Return Value
Exported DataTable object.
### Remarks
All data in the [`Cells`](../) collection are converted to strings.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Export data to DataTable
int maxRow = worksheet.Cells.MaxDataRow + 1;
int maxCol = worksheet.Cells.MaxDataColumn + 1;
DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);
// Display the exported data
foreach (DataRow row in dataTable.Rows)
{
foreach (DataColumn col in dataTable.Columns)
{
Console.Write(row[col] + "\t");
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
