##HtmlSaveOptions.IsIECompatible
HtmlSaveOptions property. Indicating whether the output HTML is compatible with IE browser. The defalut value is false
## HtmlSaveOptions.IsIECompatible property
Indicating whether the output HTML is compatible with IE browser. The defalut value is false
```csharp
public bool IsIECompatible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsIECompatibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("HTML Export Demo");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set IsIECompatible property
saveOptions.IsIECompatible = false; // Disable IE compatibility mode
// Save the workbook with HTML options
workbook.Save("HtmlExportDemo.html", saveOptions);
Console.WriteLine("HTML file saved with IsIECompatible = false");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
