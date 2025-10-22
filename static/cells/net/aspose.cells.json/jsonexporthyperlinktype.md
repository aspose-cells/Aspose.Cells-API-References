##Enum JsonExportHyperlinkType
Aspose.Cells.Json.JsonExportHyperlinkType enum. Represents type of exporting hyperlinks to json
## JsonExportHyperlinkType enumeration
Represents type of exporting hyperlinks to json.
```csharp
public enum JsonExportHyperlinkType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DisplayString | `0` | Export display string |
| Address | `1` | Export url |
| HtmlString | `2` | Export as html string. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Json;
using System;
public class JsonExportHyperlinkTypeDemo
{
public static void JsonExportHyperlinkTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data with hyperlinks
worksheet.Cells["A1"].PutValue("Google");
worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.google.com");
worksheet.Cells["A2"].PutValue("Aspose");
worksheet.Hyperlinks.Add("A2", 1, 1, "http://www.aspose.com");
// Create JsonSaveOptions and set ExportHyperlinkType
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.DisplayString;
// Save the workbook to JSON format
workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksDisplayString.json", saveOptions);
// Change ExportHyperlinkType to Address and save again
saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.Address;
workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksAddress.json", saveOptions);
// Change ExportHyperlinkType to HtmlString and save again
saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
workbook.Save("JsonExportHyperlinkTypeExample_HyperlinksHtmlString.json", saveOptions);
Console.WriteLine("Workbooks saved with different hyperlink export types.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Json](../../aspose.cells.json/)
* assembly [Aspose.Cells](../../)
