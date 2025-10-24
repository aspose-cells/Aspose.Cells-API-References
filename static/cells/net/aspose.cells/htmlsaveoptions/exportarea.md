##HtmlSaveOptions.ExportArea
HtmlSaveOptions property. Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html
## HtmlSaveOptions.ExportArea property
Gets or Sets the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omitted. Only the specified area will be exported when saving the file to html.
```csharp
public CellArea ExportArea { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data in the worksheet
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
}
}
// Set HTML save options with export area
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportArea = CellArea.CreateCellArea("B2", "D5");
// Save the workbook with specified export area
workbook.Save("output.html", options);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
