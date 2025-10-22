##PdfSaveOptions.FontEncoding
PdfSaveOptions property. Gets or sets embedded font encoding in pdf
## PdfSaveOptions.FontEncoding property
Gets or sets embedded font encoding in pdf.
```csharp
public PdfFontEncoding FontEncoding { get; set; }
```
### Remarks
Default value is Identity
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyFontEncodingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Font Encoding Test");
worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");
// Configure PDF save options with FontEncoding
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
pdfSaveOptions.DefaultFont = "Arial";
// Save the workbook to PDF
workbook.Save("output.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
