##HtmlSaveOptions.ExportPageHeaders
HtmlSaveOptions property. Indicates whether exporting page headers
## HtmlSaveOptions.ExportPageHeaders property
Indicates whether exporting page headers.
```csharp
public bool ExportPageHeaders { get; set; }
```
### Remarks
Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportPageHeadersDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set page header
worksheet.PageSetup.SetHeader(0, "Sample Header Text");
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("This is a test");
// Configure HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
SaveAsSingleFile = true,
ShowAllSheets = true,
ExportPageHeaders = true  // This is the key property being demonstrated
};
// Save the workbook as HTML
string outputPath = "output_with_headers.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file with page headers exported successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
