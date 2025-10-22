##Class PdfConverter
Aspose.Cells.LowCode.PdfConverter class. Converter for converting template file to pdf
## PdfConverter class
Converter for converting template file to pdf.
```csharp
public class PdfConverter
```
## Methods
| Name | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Converts template file to pdf |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Converts given template file to pdf. |
### Examples
```csharp
using System;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeClassPdfConverterDemo
{
public static void Run()
{
// Initialize the PdfConverter with template and output paths
PdfConverter.Process("template.xlsx", "res.pdf");
Console.WriteLine("PDF conversion completed successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
