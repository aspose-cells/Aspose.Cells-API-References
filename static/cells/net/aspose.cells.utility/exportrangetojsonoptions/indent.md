##ExportRangeToJsonOptions.Indent
ExportRangeToJsonOptions property. Indicates the indent
## ExportRangeToJsonOptions.Indent property
Indicates the indent.
```csharp
public string Indent { get; set; }
```
### Remarks
If the indent is null or empty, the exported json is not formatted.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Utility;
using System;
public class ExportRangeToJsonOptionsPropertyIndentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create ExportRangeToJsonOptions instance
ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
options.HasHeaderRow = true;
// Display current indent (default is null)
Console.WriteLine("Current Indent value: " + (options.Indent ?? "null"));
// Export with default indent (compact JSON)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
string jsonWithoutIndent = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("JSON without indent:\n" + jsonWithoutIndent);
// Set indent to 4 spaces
options.Indent = "    ";
string jsonWithIndent = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("\nJSON with 4-space indent:\n" + jsonWithIndent);
// Set indent to tab character
options.Indent = "\t";
string jsonWithTabIndent = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("\nJSON with tab indent:\n" + jsonWithTabIndent);
}
}
}
```
### See Also
* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
