##HtmlSaveOptions.IsJsBrowserCompatible
HtmlSaveOptions property. Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true
## HtmlSaveOptions.IsJsBrowserCompatible property
Indicates whether JavaScript is compatible with browsers that do not support JavaScript. The default value is true.
```csharp
public bool IsJsBrowserCompatible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");
// Configure HTML save options with IsJsBrowserCompatible set to true
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IsJsBrowserCompatible = true,
ExportFormula = true,
PresentationPreference = true
};
// Save the workbook with JavaScript compatibility
workbook.Save("JsCompatibleOutput.html", saveOptions);
Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
