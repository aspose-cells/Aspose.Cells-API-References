##HtmlSaveOptions.ExportGridLines
HtmlSaveOptions property. Indicating whether exporting the gridlines.The default value is false
## HtmlSaveOptions.ExportGridLines property
Indicating whether exporting the gridlines.The default value is false.
```csharp
public bool ExportGridLines { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportGridLinesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set gridlines visibility
worksheet.IsGridlinesVisible = true;
// Add sample data
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["B2"].PutValue(123);
worksheet.Cells["C3"].PutValue(DateTime.Now);
// Create HTML save options
HtmlSaveOptions options = new HtmlSaveOptions
{
ExportGridLines = worksheet.IsGridlinesVisible,
ExportActiveWorksheetOnly = true
};
// Save as HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with ExportGridLines: " + options.ExportGridLines);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
