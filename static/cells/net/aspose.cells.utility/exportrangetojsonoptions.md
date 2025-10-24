##Class ExportRangeToJsonOptions
Aspose.Cells.Utility.ExportRangeToJsonOptions class. Indicates the options that exporting range to json
## ExportRangeToJsonOptions class
Indicates the options that exporting range to json.
```csharp
public class ExportRangeToJsonOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Exports the string value of the cells to json. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Indicates whether exporting empty cells as null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Indicates whether the range contains header row. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Indicates the indent. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class UtilityClassExportRangeToJsonOptionsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create export options
var exportOptions = new ExportRangeToJsonOptions();
// Export range to JSON
var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
// Output the JSON
Console.WriteLine("Exported JSON:");
Console.WriteLine(jsonData);
// Save to file (optional)
File.WriteAllText("exported_data.json", jsonData);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)
