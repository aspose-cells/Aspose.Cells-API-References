##Enum HtmlLinkTargetType
Aspose.Cells.HtmlLinkTargetType enum. Represents the type of target attribute in HTML  tag
## HtmlLinkTargetType enumeration
Represents the type of target attribute in HTML  tag.
```csharp
public enum HtmlLinkTargetType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Blank | `0` | Opens the linked document in a new window or tab |
| Parent | `1` | Opens the linked document in the parent frame |
| Self | `2` | Opens the linked document in the same frame as it was clicked (this is default) |
| Top | `3` | Opens the linked document in the full body of the window |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlLinkTargetTypeDemo
{
public static void HtmlLinkTargetTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Click here to visit Aspose");
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Create HtmlSaveOptions and set the LinkTargetType
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.LinkTargetType = HtmlLinkTargetType.Blank; // Opens the link in a new window or tab
// Save the workbook to HTML format
workbook.Save("HtmlLinkTargetTypeExample.html", saveOptions);
Console.WriteLine("HTML file saved with link target type set to '_blank'.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
