##LowCodePdfSaveOptions.SaveFormat
LowCodePdfSaveOptions property. The save format for the output. For converting to pdf it can only be Pdf
## LowCodePdfSaveOptions.SaveFormat property
The save format for the output. For converting to pdf, it can only be Pdf.
```csharp
public override SaveFormat SaveFormat { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
using System;
public class LowCodePdfSaveOptionsPropertySaveFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Testing PDF SaveFormat Property");
LowCodePdfSaveOptions pdfOptions = new LowCodePdfSaveOptions();
Console.WriteLine("Current SaveFormat value: " + pdfOptions.SaveFormat);
pdfOptions.SaveFormat = SaveFormat.Pdf;
PdfSaveOptions options = pdfOptions.PdfOptions;
options.Compliance = PdfCompliance.PdfA1a;
workbook.Save("LowCodePdfSaveFormatDemo.pdf", options);
}
}
}
```
### See Also
* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
