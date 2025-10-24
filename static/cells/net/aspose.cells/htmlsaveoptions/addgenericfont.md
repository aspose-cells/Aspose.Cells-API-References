##HtmlSaveOptions.AddGenericFont
HtmlSaveOptions property. Indicates whether to add a generic font to CSS fontfamily. The default value is true
## HtmlSaveOptions.AddGenericFont property
Indicates whether to add a generic font to CSS font-family. The default value is true
```csharp
public bool AddGenericFont { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyAddGenericFontDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample text with a specific font
var cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
Style style = cell.GetStyle();
style.Font.Name = "Pacifico";
cell.SetStyle(style);
// Save with AddGenericFont enabled (default)
HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
workbook.Save("output_with_generic.html", options);
// Save with AddGenericFont disabled
options.AddGenericFont = false;
workbook.Save("output_without_generic.html", options);
// Verify the results
string withGeneric = File.ReadAllText("output_with_generic.html");
string withoutGeneric = File.ReadAllText("output_without_generic.html");
Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
