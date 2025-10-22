##ExportRangeToJsonOptions.HasHeaderRow
ExportRangeToJsonOptions property. Indicates whether the range contains header row
## ExportRangeToJsonOptions.HasHeaderRow property
Indicates whether the range contains header row.
```csharp
public bool HasHeaderRow { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Utility;
using System;
public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data with headers
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["B3"].PutValue(25);
// Create range to export
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
// Create ExportRangeToJsonOptions instance
ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
// Display current HasHeaderRow value (default is false)
Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);
// Set HasHeaderRow to true
options.HasHeaderRow = true;
Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);
// Export to JSON with headers
string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);
// Set HasHeaderRow to false
options.HasHeaderRow = false;
Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);
// Export to JSON without headers
string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);
// Save the workbook
workbook.Save("PropertyHasHeaderRowDemo.xlsx");
}
}
}
```
### See Also
* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
