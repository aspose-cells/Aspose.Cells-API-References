##Cells.ImportDataView
Cells method. Imports a DataView into a worksheet
## Cells.ImportDataView method
Imports a DataView into a worksheet.
```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
### Return Value
Total number of rows imported
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportDataViewWithDataViewInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample DataTable
DataTable table = new DataTable("Products");
table.Columns.Add("ID", typeof(int));
table.Columns.Add("Name", typeof(string));
table.Columns.Add("Price", typeof(decimal));
// Add sample data
table.Rows.Add(1, "Laptop", 999.99m);
table.Rows.Add(2, "Smartphone", 699.99m);
table.Rows.Add(3, "Tablet", 399.99m);
// Create DataView from DataTable
DataView dataView = new DataView(table);
// Import DataView into worksheet starting at row 0, column 0
cells.ImportDataView(dataView, 0, 0);
// Save the workbook
workbook.Save("ImportDataViewOutput.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
