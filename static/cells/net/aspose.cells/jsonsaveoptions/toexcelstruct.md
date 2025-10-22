##JsonSaveOptions.ToExcelStruct
JsonSaveOptions property. Indicates whether converting to json struct of the Excel file
## JsonSaveOptions.ToExcelStruct property
Indicates whether converting to json struct of the Excel file.
```csharp
public bool ToExcelStruct { get; set; }
```
### Remarks
Only for converting range to JSON.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyToExcelStructDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Create a range to export
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
// Configure JSON save options with ToExcelStruct
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.AlwaysExportAsJsonObject = true;
saveOptions.ToExcelStruct = true;
// Export range to JSON
string json = range.ToJson(saveOptions);
Console.WriteLine(json);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
