##HtmlSaveOptions.ExportPrintAreaOnly
HtmlSaveOptions property. Indicates if only exporting the print area to html file. The default value is false
## HtmlSaveOptions.ExportPrintAreaOnly property
Indicates if only exporting the print area to html file. The default value is false.
```csharp
public bool ExportPrintAreaOnly { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
for (int i = 0; i < 20; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
}
}
// Set print area
worksheet.PageSetup.PrintArea = "B2:F10";
// Configure HTML save options
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportPrintAreaOnly = true;
options.ExportGridLines = true;
// Save the workbook with print area only
workbook.Save("output.html", options);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
