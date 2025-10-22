##ImportTableOptions.ColumnIndexes
ImportTableOptions property. Gets or sets the columns0based to import from data source. null means all columns should be imported
## ImportTableOptions.ColumnIndexes property
Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.
```csharp
public int[] ColumnIndexes { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyColumnIndexesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample DataTable
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Name", typeof(string));
dataTable.Columns.Add("Price", typeof(decimal));
// Add sample data
dataTable.Rows.Add(1, "Product A", 19.99m);
dataTable.Rows.Add(2, "Product B", 29.99m);
dataTable.Rows.Add(3, "Product C", 39.99m);
// Set import options to only import columns at indexes 0 and 2 (ID and Price)
ImportTableOptions options = new ImportTableOptions();
options.ColumnIndexes = new int[] { 0, 2 };
options.IsFieldNameShown = true;
// Import data with specified column indexes
worksheet.Cells.ImportData(dataTable, 0, 0, options);
// Save the workbook
workbook.Save("ColumnIndexesDemo.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
