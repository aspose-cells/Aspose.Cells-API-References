##PdfSaveOptions.Compliance
PdfSaveOptions property. Gets or sets the PDF standards compliance level for output documents
## PdfSaveOptions.Compliance property
Gets or sets the PDF standards compliance level for output documents.
```csharp
public PdfCompliance Compliance { get; set; }
```
### Remarks
Default is Pdf17.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyComplianceDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test PDF Compliance");
// Set PDF save options with PDF/A-1b compliance
PdfSaveOptions options = new PdfSaveOptions
{
Compliance = PdfCompliance.PdfA1b
};
// Save the workbook as PDF with compliance settings
workbook.Save("output.pdf", options);
Console.WriteLine("PDF saved with PDF/A-1b compliance.");
}
}
}
```
### See Also
* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
