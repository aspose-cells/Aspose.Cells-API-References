##ExportRangeToJsonOptions.ExportEmptyCells
ExportRangeToJsonOptions property. Indicates whether exporting empty cells as null
## ExportRangeToJsonOptions.ExportEmptyCells property
Indicates whether exporting empty cells as null.
```csharp
public bool ExportEmptyCells { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
// Leave B2 empty intentionally
// Create export options and enable exporting empty cells
ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
exportOptions.ExportEmptyCells = true;
// Export the range to JSON
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
Console.WriteLine(jsonData);
}
}
}
```
### See Also
* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
