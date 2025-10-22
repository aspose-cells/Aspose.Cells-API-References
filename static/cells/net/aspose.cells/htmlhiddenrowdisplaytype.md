##Enum HtmlHiddenRowDisplayType
Aspose.Cells.HtmlHiddenRowDisplayType enum. Represents two types of showing the hidden rows in html
## HtmlHiddenRowDisplayType enumeration
Represents two types of showing the hidden rows in html.
```csharp
public enum HtmlHiddenRowDisplayType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Hidden | `0` | Hidden the hidden rows in html page. |
| Remove | `1` | Remove the hidden rows in html page. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlHiddenRowDisplayTypeDemo
{
public static void HtmlHiddenRowDisplayTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Visible Row");
worksheet.Cells["A2"].PutValue("Hidden Row");
worksheet.Cells["A3"].PutValue("Another Visible Row");
// Hide the second row
worksheet.Cells.HideRow(1);
// Create HtmlSaveOptions and set the HiddenRowDisplayType
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove
// Save the workbook to HTML format
workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);
Console.WriteLine("Workbook saved as HTML with hidden row display type.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
