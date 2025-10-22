##HtmlSaveOptions.HtmlSaveOptions
HtmlSaveOptions constructor. Creates options for saving html file
## HtmlSaveOptions() {#constructor}
Creates options for saving html file.
```csharp
public HtmlSaveOptions()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample HTML Export");
// Initialize HtmlSaveOptions using constructor
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportActiveWorksheetOnly = true;
// Save as HTML
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file saved to: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## HtmlSaveOptions(SaveFormat) {#constructor_1}
Creates options for saving htm file.
```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Html or MHtml, otherwise the saved format will be set as Html automatically. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlSaveOptionsMethodCtorWithSaveFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to worksheet
worksheet.Cells["A1"].PutValue("Sample HTML Export");
worksheet.Cells["B2"].PutValue(123.45);
worksheet.Cells["C3"].PutValue(DateTime.Now);
try
{
// Create HtmlSaveOptions with SaveFormat parameter
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
// Set some properties
saveOptions.PageTitle = "Aspose.Cells HTML Export";
saveOptions.ExportActiveWorksheetOnly = true;
saveOptions.ExportGridLines = true;
// Save workbook with HtmlSaveOptions
workbook.Save("HtmlExportWithOptions.html", saveOptions);
Console.WriteLine("HTML file saved successfully with HtmlSaveOptions(SaveFormat)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing HtmlSaveOptions constructor: {ex.Message}");
}
}
}
}
```
### See Also
* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
