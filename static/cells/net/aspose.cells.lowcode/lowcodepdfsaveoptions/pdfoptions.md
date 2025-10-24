##LowCodePdfSaveOptions.PdfOptions
LowCodePdfSaveOptions property. The options for saving Pdf file
## LowCodePdfSaveOptions.PdfOptions property
The options for saving Pdf file.
```csharp
public PdfSaveOptions PdfOptions { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodePdfSaveOptionsPropertyPdfOptionsDemo
{
public static void Run()
{
// Create sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("PDF Options Demo");
// Create PDF save options with custom settings
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
{
Compliance = PdfCompliance.PdfA1b,
OnePagePerSheet = true
};
// Create low code PDF save options and assign the PDF options
LowCodePdfSaveOptions lowCodePdfSaveOptions = new LowCodePdfSaveOptions
{
OutputFile = "output.pdf",
PdfOptions = pdfSaveOptions
};
// Save using low code options
workbook.Save(lowCodePdfSaveOptions.OutputFile, lowCodePdfSaveOptions.PdfOptions);
Console.WriteLine("PDF saved with custom options.");
}
}
}
```
### See Also
* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
