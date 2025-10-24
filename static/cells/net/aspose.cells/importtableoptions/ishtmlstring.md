##ImportTableOptions.IsHtmlString
ImportTableOptions property. Indicates whether the value contains html tags
## ImportTableOptions.IsHtmlString property
Indicates whether the value contains html tags.
```csharp
public bool IsHtmlString { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ImportTableOptionsPropertyIsHtmlStringDemo
{
public static void Run()
{
// Create a DataTable with sample data containing HTML
DataTable table = new DataTable();
table.Columns.Add("ID");
table.Columns.Add("Content");
table.Columns.Add("Time");
// Add a row with HTML content
table.Rows.Add("1", "<a href='https://www.example.com'>Example Link</a>", "2:30 PM");
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Import the DataTable with IsHtmlString set to true
worksheet.Cells.ImportData(table, 0, 0, new ImportTableOptions
{
IsFieldNameShown = true,
IsHtmlString = true,
NumberFormats = new string[] { null, null, "h:mm AM/PM" }
});
// Save the workbook
workbook.Save("HtmlStringImportDemo.xlsx");
}
}
}
```
### See Also
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
