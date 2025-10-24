##ImportTableOptions.ConvertGridStyle
ImportTableOptions property. Indicates whether apply the style of the grid view to cells
## ImportTableOptions.ConvertGridStyle property
Indicates whether apply the style of the grid view to cells.
```csharp
public bool ConvertGridStyle { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyConvertGridStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
DataTable dataTable = new DataTable("Products");
dataTable.Columns.Add("ID", typeof(int));
dataTable.Columns.Add("Product", typeof(string));
dataTable.Columns.Add("Price", typeof(decimal));
dataTable.Rows.Add(101, "Laptop", 999.99m);
dataTable.Rows.Add(102, "Monitor", 249.50m);
// Set import options with ConvertGridStyle enabled
ImportTableOptions options = new ImportTableOptions();
options.ConvertGridStyle = true; // This will apply grid styling to the imported data
options.IsFieldNameShown = true;
// Import data with styling
worksheet.Cells.ImportData(dataTable, 0, 0, options);
// Save the result
workbook.Save("ImportWithGridStyle.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
