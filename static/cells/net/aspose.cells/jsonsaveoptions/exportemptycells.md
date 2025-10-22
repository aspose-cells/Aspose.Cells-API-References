##JsonSaveOptions.ExportEmptyCells
JsonSaveOptions property. Indicates whether exporting empty cells as null
## JsonSaveOptions.ExportEmptyCells property
Indicates whether exporting empty cells as null.
```csharp
public bool ExportEmptyCells { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyExportEmptyCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill data with some empty cells
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty
// Create JsonSaveOptions with ExportEmptyCells set to false
JsonSaveOptions options = new JsonSaveOptions
{
ExportEmptyCells = false
};
// Save to JSON - empty cells will be skipped
workbook.Save("output_skip_empty.json", options);
// Change ExportEmptyCells to true
options.ExportEmptyCells = true;
// Save again - empty cells will be included
workbook.Save("output_include_empty.json", options);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
