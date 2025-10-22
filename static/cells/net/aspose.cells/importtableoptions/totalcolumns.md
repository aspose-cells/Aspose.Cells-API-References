##ImportTableOptions.TotalColumns
ImportTableOptions property. Gets or sets total column count to import from data source. 1 means all rows of given data source
## ImportTableOptions.TotalColumns property
Gets or sets total column count to import from data source. -1 means all rows of given data source.
```csharp
public int TotalColumns { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyTotalColumnsDemo
{
public static void Run()
{
// Create a sample DataTable
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Name", typeof(string));
dataTable.Columns.Add("Price", typeof(decimal));
// Add sample data
dataTable.Rows.Add(1, "Product A", 19.99m);
dataTable.Rows.Add(2, "Product B", 29.99m);
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set import options with TotalColumns = 2 (will only import first 2 columns)
ImportTableOptions importOptions = new ImportTableOptions
{
IsFieldNameShown = true,
TotalColumns = 2 // Only import first 2 columns (ID and Name)
};
// Import data starting from cell A1
cells.ImportData(dataTable, 0, 0, importOptions);
// Save the workbook
workbook.Save("ImportWithTotalColumns.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Data imported with TotalColumns=2. Only first 2 columns were imported.");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
