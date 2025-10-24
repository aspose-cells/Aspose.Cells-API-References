##ImportTableOptions.DateFormat
ImportTableOptions property. Gets or sets date format string for cells with imported datetime values
## ImportTableOptions.DateFormat property
Gets or sets date format string for cells with imported datetime values.
```csharp
public string DateFormat { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyDateFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a sample DataTable with date values
DataTable dataTable = new DataTable();
dataTable.Columns.Add("DateColumn", typeof(DateTime));
dataTable.Rows.Add(new DateTime(2023, 1, 15));
dataTable.Rows.Add(new DateTime(2023, 2, 20));
dataTable.Rows.Add(new DateTime(2023, 3, 25));
// Define the import range
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);
// Import data with custom date format
worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
{
IsFieldNameShown = true,
DateFormat = "YYYY-MM-DD"
});
// Save the workbook to demonstrate the result
workbook.Save("DateFormatDemoOutput.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
