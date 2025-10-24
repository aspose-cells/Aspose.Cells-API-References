##HtmlSaveOptions.IsMobileCompatible
HtmlSaveOptions property. Indicates whether the output HTML is compatible with mobile devices. The default value is false
## HtmlSaveOptions.IsMobileCompatible property
Indicates whether the output HTML is compatible with mobile devices. The default value is false.
```csharp
public bool IsMobileCompatible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set mobile compatibility
saveOptions.IsMobileCompatible = true;
// Save with mobile compatibility enabled
workbook.Save("MobileCompatible.html", saveOptions);
// Change to non-mobile compatible
saveOptions.IsMobileCompatible = false;
workbook.Save("NonMobileCompatible.html", saveOptions);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
