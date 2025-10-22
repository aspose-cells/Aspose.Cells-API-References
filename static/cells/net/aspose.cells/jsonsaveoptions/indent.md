##JsonSaveOptions.Indent
JsonSaveOptions property. Indicates the indent
## JsonSaveOptions.Indent property
Indicates the indent.
```csharp
public string Indent { get; set; }
```
### Remarks
If the indent is null or empty, the exported json is not formatted.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyIndentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["B3"].PutValue(25);
// Configure JSON save options with indentation
JsonSaveOptions saveOptions = new JsonSaveOptions
{
Indent = "    ", // 4 spaces for indentation
ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
HasHeaderRow = true
};
// Save with indented JSON output
workbook.Save("IndentedJsonOutput.json", saveOptions);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
