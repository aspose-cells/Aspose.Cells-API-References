##Enum PdfCompressionCore
Aspose.Cells.Rendering.PdfCompressionCore enum. Specifies a type of compression applied to all content in the PDF file except images
## PdfCompressionCore enumeration
Specifies a type of compression applied to all content in the PDF file except images.
```csharp
public enum PdfCompressionCore
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | None |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfCompressionCoreDemo
{
public static void PdfCompressionCoreExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello Aspose!");
// Create PdfSaveOptions and set the PdfCompressionCore
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate
// Save the workbook as a PDF file with the specified compression
workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);
Console.WriteLine("PDF file saved with specified compression.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
