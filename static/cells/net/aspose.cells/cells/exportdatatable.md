##Cells.ExportDataTable
Cells method. Exports data in the Cells collection to a DataTable object
## ExportDataTable(int, int, int, int) {#exportdatatable}
Exports data in the [`Cells`](../) collection to a DataTable object.
```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
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
If you use this method to export a block of data, please be sure that the data in a column should be the same data type. Otherwise, use the [`ExportDataTableAsString`](../exportdatatableasstring/) method instead.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["C1"].PutValue("City");
for (int i = 1; i <= 5; i++)
{
worksheet.Cells[i, 0].PutValue($"Person {i}");
worksheet.Cells[i, 1].PutValue(20 + i);
worksheet.Cells[i, 2].PutValue($"City {i}");
}
// Export data to DataTable (starting from row 0, column 0, with 5 rows and 3 columns)
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);
// Display the exported data
Console.WriteLine("Exported DataTable:");
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}
Exports data in the [`Cells`](../) collection to a DataTable object.
```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns,
bool exportColumnName)
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
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
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
// Export data to DataTable (first row contains headers)
DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);
// Display the exported data
Console.WriteLine("Exported DataTable:");
foreach (DataRow row in dt.Rows)
{
Console.WriteLine($"{row["Name"]}, {row["Age"]}");
}
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}
Exports data in the [`Cells`](../) collection to a DataTable object.
```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns,
ExportTableOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be imported. |
| totalColumns | Int32 | Number of columns to be imported. |
| options | ExportTableOptions | All export table options |
### Return Value
Exported DataTable object.
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set value and format for cell A1
cells["A1"].PutValue(1.23356);
Style style = cells["A1"].GetStyle();
style.Custom = "0.00";
cells["A1"].SetStyle(style);
// Create export options
ExportTableOptions etOpt = new ExportTableOptions();
etOpt.ExportColumnName = false;
etOpt.ExportAsString = true;
// Export with CellStyle format strategy
etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());
// Export with None format strategy
etOpt.FormatStrategy = CellValueFormatStrategy.None;
DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());
// Export with DisplayStyle format strategy
etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
}
}
}
```
### See Also
* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
