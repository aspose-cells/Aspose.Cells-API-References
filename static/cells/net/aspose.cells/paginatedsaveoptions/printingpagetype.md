##PaginatedSaveOptions.PrintingPageType
PaginatedSaveOptions property. Indicates which pages will not be printed
## PaginatedSaveOptions.PrintingPageType property
Indicates which pages will not be printed.
```csharp
public PrintingPageType PrintingPageType { get; set; }
```
### Remarks
If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add some sample data
ws.Cells["A1"].PutValue("Sample Data");
ws.Cells["A2"].PutValue(123);
ws.Cells["A3"].PutValue(456);
// Create blank worksheet
Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Save ignoring blank pages
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
// Save ignoring blank pages and style-only pages
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
