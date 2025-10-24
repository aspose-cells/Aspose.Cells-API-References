##Enum PdfFontEncoding
Aspose.Cells.Rendering.PdfFontEncoding enum. Represents pdf embedded font encoding
## PdfFontEncoding enumeration
Represents pdf embedded font encoding.
```csharp
public enum PdfFontEncoding
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Identity | `0` | Represents use Identity-H encoding for all embedded fonts in pdf. |
| AnsiPrefer | `1` | Represents prefer to use WinAnsiEncoding for TrueType fonts with characters 32-127, otherwise, Identity-H encoding will be used for embedded fonts in pdf. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfFontEncodingDemo
{
public static void PdfFontEncodingExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello, Aspose!");
// Create PdfSaveOptions and set the FontEncoding property
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;
// Save the workbook as a PDF file
workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);
Console.WriteLine("PDF file created successfully with specified font encoding.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
