##ImportTableOptions.InsertRows
ImportTableOptions property. Indicates whether new rows should be added for importing data records
## ImportTableOptions.InsertRows property
Indicates whether new rows should be added for importing data records.
```csharp
public bool InsertRows { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyInsertRowsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data table
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Product", typeof(string));
dataTable.Columns.Add("Price", typeof(decimal));
dataTable.Rows.Add(1, "Laptop", 999.99);
dataTable.Rows.Add(2, "Monitor", 249.99);
dataTable.Rows.Add(3, "Keyboard", 49.99);
// Add existing data to worksheet (will be shifted down by insert)
cells["A1"].PutValue("Existing Data");
cells["A2"].PutValue(100);
// Set import options with InsertRows = true
ImportTableOptions options = new ImportTableOptions();
options.InsertRows = true; // This will insert new rows instead of overwriting
options.IsFieldNameShown = true;
// Import data starting at row 1 (will insert rows below existing data)
cells.ImportData(dataTable, 1, 0, options);
// Save the workbook
workbook.Save("InsertRowsDemo.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
