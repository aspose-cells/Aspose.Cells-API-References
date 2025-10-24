##HtmlSaveOptions.HtmlVersion
HtmlSaveOptions property. Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default
## HtmlSaveOptions.HtmlVersion property
Specifies version of HTML standard that should be used when saving the HTML format. Default value is HtmlVersion.Default.
```csharp
public HtmlVersion HtmlVersion { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlSaveOptionsPropertyHtmlVersionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("HTML Version Demo");
worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
worksheet.Cells["B3"].PutValue(123.45);
worksheet.Cells["C4"].PutValue("Sample Text");
// Create HtmlSaveOptions instance
HtmlSaveOptions options = new HtmlSaveOptions();
// Display current HtmlVersion value
Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
// Set HtmlVersion to HTML5
options.HtmlVersion = HtmlVersion.Html5;
Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
// Save with HTML5 version
workbook.Save("HtmlVersion_Html5.html", options);
// Change to XHTML
options.HtmlVersion = HtmlVersion.XHtml;
Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
// Save with XHTML version
workbook.Save("HtmlVersion_XHtml.html", options);
// Reset to default
options.HtmlVersion = HtmlVersion.Default;
Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
// Save with default version
workbook.Save("HtmlVersion_Default.html", options);
}
}
}
```
### See Also
* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
