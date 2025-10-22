##PdfSaveOptions.PdfCompression
PdfSaveOptions property. Indicate the compression algorithm
## PdfSaveOptions.PdfCompression property
Indicate the compression algorithm
```csharp
public PdfCompressionCore PdfCompression { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyPdfCompressionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
// Create PDF save options with Flate compression
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PdfCompression = PdfCompressionCore.Flate;
// Save the workbook as PDF with compression
workbook.Save("output_with_flate_compression.pdf", saveOptions);
// Save again with no compression for comparison
saveOptions.PdfCompression = PdfCompressionCore.None;
workbook.Save("output_without_compression.pdf", saveOptions);
Console.WriteLine("PDF files created successfully with different compression settings.");
}
}
}
```
### See Also
* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
