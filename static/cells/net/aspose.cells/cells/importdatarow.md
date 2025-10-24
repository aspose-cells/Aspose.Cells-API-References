##Cells.ImportDataRow
Cells method. Imports a DataRow into the Excel file
## Cells.ImportDataRow method
Imports a DataRow into the Excel file.
```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataRow | DataRow | DataRow object. |
| row | Int32 | Row index. |
| firstColumn | Int32 | First column index. |
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportDataRowWithDataRowInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a sample DataTable
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Name", typeof(string));
dataTable.Columns.Add("Price", typeof(decimal));
// Add sample data
dataTable.Rows.Add(1, "Product A", 19.99m);
dataTable.Rows.Add(2, "Product B", 29.99m);
// Import the first row from DataTable to worksheet starting at row 0, column 0
cells.ImportDataRow(dataTable.Rows[0], 0, 0);
// Save the workbook
workbook.Save("ImportDataRowDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
