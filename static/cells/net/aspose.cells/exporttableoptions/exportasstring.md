##ExportTableOptions.ExportAsString
ExportTableOptions property. Exports the string value of the cells to the DataTable
## ExportTableOptions.ExportAsString property
Exports the string value of the cells to the DataTable.
```csharp
public bool ExportAsString { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExportTableOptionsPropertyExportAsStringDemo
{
public static void Run()
{
// Create a new workbook and get the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with mixed types
worksheet.Cells[0, 0].PutValue("ID");
worksheet.Cells[0, 1].PutValue("Value");
worksheet.Cells[1, 0].PutValue(1);
worksheet.Cells[1, 1].PutValue(123.45);
worksheet.Cells[2, 0].PutValue(2);
worksheet.Cells[2, 1].PutValue("TextValue");
// Create export options with ExportAsString set to true
ExportTableOptions exportOptions = new ExportTableOptions
{
ExportColumnName = true,
ExportAsString = true // This forces all values to be exported as strings
};
// Export data to DataTable
DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);
// Display the exported data types
Console.WriteLine("Data exported with ExportAsString=true:");
foreach (DataRow row in dataTable.Rows)
{
Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
}
// Now export with ExportAsString=false
exportOptions.ExportAsString = false;
DataTable dataTable2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);
Console.WriteLine("\nData exported with ExportAsString=false:");
foreach (DataRow row in dataTable2.Rows)
{
Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
}
}
}
}
```
### See Also
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
