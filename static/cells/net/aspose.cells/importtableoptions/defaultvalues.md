##ImportTableOptions.DefaultValues
ImportTableOptions property. Default value for the value in the table is null
## ImportTableOptions.DefaultValues property
Default value for the value in the table is null.
```csharp
public object[] DefaultValues { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Data;
public class ImportTableOptionsPropertyDefaultValuesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data with null values
DataTable dataTable = new DataTable();
dataTable.Columns.Add("Product", typeof(string));
dataTable.Columns.Add("Quantity", typeof(int));
dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
dataTable.Rows.Add(null, null, null); // Will use default values
dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));
ImportTableOptions importOptions = new ImportTableOptions();
// Display initial state
Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));
// Configure default values for each column
importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };
// Import data with null handling
worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);
// Auto-fit columns for better visibility
worksheet.AutoFitColumns();
workbook.Save("DefaultValuesDemo.xlsx");
Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
