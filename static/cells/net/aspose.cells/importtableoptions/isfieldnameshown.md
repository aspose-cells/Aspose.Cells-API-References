##ImportTableOptions.IsFieldNameShown
ImportTableOptions property. Indicates whether field name should be imported
## ImportTableOptions.IsFieldNameShown property
Indicates whether field name should be imported.
```csharp
public bool IsFieldNameShown { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyIsFieldNameShownDemo
{
public static void Run()
{
// Create a sample DataTable
DataTable table = new DataTable();
table.Columns.Add("ID");
table.Columns.Add("Product");
// Add sample data
table.Rows.Add(1, "Laptop");
table.Rows.Add(2, "Smartphone");
table.Rows.Add(3, "Tablet");
// Create a workbook and import data with field names shown
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
ImportTableOptions options = new ImportTableOptions();
options.IsFieldNameShown = true;  // Show field names
options.InsertRows = true;       // Insert new rows
// Import data starting from row 5, column 0
cells.ImportData(table, 5, 0, options);
// Save the workbook
workbook.Save("ImportDataWithFieldNames.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
