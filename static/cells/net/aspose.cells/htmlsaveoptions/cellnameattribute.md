##HtmlSaveOptions.CellNameAttribute
HtmlSaveOptions property. Specifies the attribute that indicates the CellName to be written. e.g. If the value is id then for cell A1 the output will betd idA1. The default value is null
## HtmlSaveOptions.CellNameAttribute property
Specifies the attribute that indicates the CellName to be written. (e.g. If the value is "id", then for cell "A1", the output will be:&lt;td id='A1'&gt;). The default value is null.
```csharp
public string CellNameAttribute { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyCellNameAttributeDemo
{
public static void Run()
{
// Create a sample workbook with some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Data");
worksheet.Cells["B2"].PutValue(123);
// Set HTML save options with CellNameAttribute
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.CellNameAttribute = "id";
saveOptions.ExportImagesAsBase64 = true;
saveOptions.ExportActiveWorksheetOnly = true;
// Save to HTML file
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
// Verify the HTML output contains cell IDs
string htmlContent = File.ReadAllText(outputPath);
Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
