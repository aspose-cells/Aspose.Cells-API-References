##JsonSaveOptions.ExportArea
JsonSaveOptions property. Gets or sets the exporting range
## JsonSaveOptions.ExportArea property
Gets or sets the exporting range.
```csharp
public CellArea ExportArea { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyExportAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["B3"].PutValue(25);
// Configure JSON save options with ExportArea
JsonSaveOptions saveOptions = new JsonSaveOptions
{
ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
};
// Save with specified export area (A1:B3)
workbook.Save("JsonExportAreaDemo.json", saveOptions);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
