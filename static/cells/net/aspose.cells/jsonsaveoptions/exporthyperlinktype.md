##JsonSaveOptions.ExportHyperlinkType
JsonSaveOptions property. Represents the type of exporting hyperlink to json
## JsonSaveOptions.ExportHyperlinkType property
Represents the type of exporting hyperlink to json.
```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```
### Remarks
The default value is DisplayString;
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a hyperlink to cell A1
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
// Set export options for JSON
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
// Save workbook to JSON
string outputPath = "output.json";
workbook.Save(outputPath, saveOptions);
// Verify the output contains the hyperlink
string jsonContent = File.ReadAllText(outputPath);
Console.WriteLine("JSON content contains hyperlink: " +
jsonContent.Contains("https://www.aspose.com"));
}
}
}
```
### See Also
* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
