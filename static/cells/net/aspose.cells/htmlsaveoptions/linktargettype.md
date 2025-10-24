##HtmlSaveOptions.LinkTargetType
HtmlSaveOptions property. Indicating the type of target attribute in a link. The default value is HtmlLinkTargetType.Parent
## HtmlSaveOptions.LinkTargetType property
Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent.
```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Link to Google");
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");
// Set HTML save options with LinkTargetType
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
// Save the workbook as HTML
workbook.Save("output.html", saveOptions);
}
}
}
```
### See Also
* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
