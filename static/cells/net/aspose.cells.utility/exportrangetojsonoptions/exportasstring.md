##ExportRangeToJsonOptions.ExportAsString
ExportRangeToJsonOptions property. Exports the string value of the cells to json
## ExportRangeToJsonOptions.ExportAsString property
Exports the string value of the cells to json.
```csharp
public bool ExportAsString { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Utility;
using System;
public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with different data types
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("String");
worksheet.Cells["B2"].PutValue("Hello");
worksheet.Cells["A3"].PutValue("Number");
worksheet.Cells["B3"].PutValue(123.45);
worksheet.Cells["A4"].PutValue("Date");
worksheet.Cells["B4"].PutValue(DateTime.Now);
// Create ExportRangeToJsonOptions instance
ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
options.HasHeaderRow = true;
// Display current ExportAsString value
Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);
// Export without ExportAsString (default behavior)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);
// Set ExportAsString to true
options.ExportAsString = true;
// Export with ExportAsString
string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);
// Save the workbook
workbook.Save("ExportAsStringDemo.xlsx");
}
}
}
```
### See Also
* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
