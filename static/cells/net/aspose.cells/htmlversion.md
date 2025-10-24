##Enum HtmlVersion
Aspose.Cells.HtmlVersion enum. Indicates the version of HTML is used when saving to Html formats
## HtmlVersion enumeration
Indicates the version of HTML is used when saving to Html formats.
```csharp
public enum HtmlVersion
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Save the document in compliance with the MS Excel exporting HTML. |
| XHtml | `1` | Saves the document in compliance with the XHTML 1.0 Transitional standard. |
| Html5 | `2` | Saves the document in compliance with the HTML 5 standard. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsClassHtmlVersionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("HTML Version Demo");
worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set HTML version to HTML5
saveOptions.HtmlVersion = HtmlVersion.Html5;
// Save the workbook with HTML5 version
workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);
// Change HTML version to XHTML
saveOptions.HtmlVersion = HtmlVersion.XHtml;
// Save the workbook with XHTML version
workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);
// Set HTML version to Default (MS Excel compatible)
saveOptions.HtmlVersion = HtmlVersion.Default;
// Save the workbook with Default version
workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
