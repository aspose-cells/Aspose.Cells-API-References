##Enum HtmlExportDataOptions
Aspose.Cells.HtmlExportDataOptions enum. Represents the options for exporting html data
## HtmlExportDataOptions enumeration
Represents the options for exporting html data.
```csharp
public enum HtmlExportDataOptions
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Table | `1` | Export file to html which only contains table part. |
| All | `255` | Export all the data to html. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlExportDataOptionsDemo
{
public static void HtmlExportDataOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John Doe");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Jane Doe");
worksheet.Cells["B3"].PutValue(25);
// Create HtmlSaveOptions and set the HtmlExportDataOptions
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML
// Save the workbook to HTML format
workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);
// Change the HtmlExportDataOptions to export only the table part
saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part
// Save the workbook to HTML format again
workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);
Console.WriteLine("HTML files have been saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
