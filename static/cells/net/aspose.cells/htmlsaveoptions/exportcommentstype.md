##HtmlSaveOptions.ExportCommentsType
HtmlSaveOptions property. Represents type of exporting comments to html files
## HtmlSaveOptions.ExportCommentsType property
Represents type of exporting comments to html files.
```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample comment using cell name
Comment comment = worksheet.Comments["A1"];
comment.Note = "This is a test comment";
// Set HTML save options with ExportCommentsType
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
// Save to HTML
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML file with comments exported successfully.");
}
}
}
```
### See Also
* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
