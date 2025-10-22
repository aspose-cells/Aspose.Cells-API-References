##ImportTableOptions.TotalRows
ImportTableOptions property. Gets or sets total row count to import from data source. 1 means all rows of given data source
## ImportTableOptions.TotalRows property
Gets or sets total row count to import from data source. -1 means all rows of given data source.
```csharp
public int TotalRows { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyTotalRowsDemo
{
public static void Run()
{
// Create a sample DataTable
DataTable table = new DataTable("TestTable");
table.Columns.Add("Column1", typeof(string));
table.Columns.Add("Column2", typeof(int));
// Add sample data
table.Rows.Add("Item1", 100);
table.Rows.Add("Item2", 200);
table.Rows.Add("Item3", 300);
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create ImportTableOptions with TotalRows set to 2 (will import only first 2 rows)
ImportTableOptions options = new ImportTableOptions
{
IsFieldNameShown = true,
TotalRows = 2 // Only import 2 rows from the DataTable
};
// Import data with the specified options
worksheet.Cells.ImportData(table, 0, 0, options);
// Save the workbook
workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
