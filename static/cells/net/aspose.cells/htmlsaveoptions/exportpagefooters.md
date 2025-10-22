##HtmlSaveOptions.ExportPageFooters
HtmlSaveOptions property. Indicates whether exporting page headers
## HtmlSaveOptions.ExportPageFooters property
Indicates whether exporting page headers.
```csharp
public bool ExportPageFooters { get; set; }
```
### Remarks
Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportPageFootersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Data");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set ExportPageFooters to true to include page footers in the output
saveOptions.ExportPageFooters = true;
// Set other necessary options
saveOptions.ExportPageHeaders = true;
// Save the workbook to HTML
workbook.Save("HtmlWithPageFooters.html", saveOptions);
Console.WriteLine("HTML file with page footers exported successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
