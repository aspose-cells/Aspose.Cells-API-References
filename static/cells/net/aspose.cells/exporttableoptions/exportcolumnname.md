##ExportTableOptions.ExportColumnName
ExportTableOptions property. Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false
## ExportTableOptions.ExportColumnName property
Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false.
```csharp
public bool ExportColumnName { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyExportColumnNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data in worksheet
cells["A1"].PutValue("Column1");
cells["B1"].PutValue("Column2");
cells["A2"].PutValue(100);
cells["B2"].PutValue("Data1");
cells["A3"].PutValue(200);
cells["B3"].PutValue("Data2");
// Configure export options
ExportTableOptions options = new ExportTableOptions();
options.ExportColumnName = true; // Demonstrating ExportColumnName property
options.IsVertical = true;
options.Indexes = new int[] { 0, 1 }; // Export all columns
// Export data from worksheet to DataTable
DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);
// Display exported data
Console.WriteLine("Exported DataTable:");
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
