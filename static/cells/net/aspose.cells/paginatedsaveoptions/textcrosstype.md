##PaginatedSaveOptions.TextCrossType
PaginatedSaveOptions property. Gets or sets displaying text type when the text width is larger than cell width
## PaginatedSaveOptions.TextCrossType property
Gets or sets displaying text type when the text width is larger than cell width.
```csharp
public TextCrossType TextCrossType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set long text that will cross cell boundaries
worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
worksheet.Cells["B1"].PutValue("Another cell content");
// Set column width to make text cross cells
worksheet.Cells.SetColumnWidth(0, 5);
// Create PDF save options
PdfSaveOptions options = new PdfSaveOptions();
// Demonstrate TextCrossType by setting it to CrossKeep
options.TextCrossType = TextCrossType.CrossKeep;
// Save the workbook as PDF
workbook.Save("TextCrossTypeDemo.pdf", options);
Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
}
}
}
```
### See Also
* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
