##JsonSaveOptions.HasHeaderRow
JsonSaveOptions property. Indicates whether the range contains header row
## JsonSaveOptions.HasHeaderRow property
Indicates whether the range contains header row.
```csharp
public bool HasHeaderRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyHasHeaderRowDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add header row
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
// Add data rows
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create range (A1:B3)
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
// Export to JSON with HasHeaderRow = true (default)
JsonSaveOptions options1 = new JsonSaveOptions();
options1.HasHeaderRow = true;
string jsonWithHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options1);
Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);
// Export to JSON with HasHeaderRow = false
JsonSaveOptions options2 = new JsonSaveOptions();
options2.HasHeaderRow = false;
string jsonWithoutHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options2);
Console.WriteLine("\nJSON without headers:\n" + jsonWithoutHeaders);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
