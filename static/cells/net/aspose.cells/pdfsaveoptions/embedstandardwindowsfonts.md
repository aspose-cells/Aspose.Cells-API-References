##PdfSaveOptions.EmbedStandardWindowsFonts
PdfSaveOptions property. True to embed true type fonts. Affects only ASCII characters 32127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A1a PDF/A1b standard. Default is true
## PdfSaveOptions.EmbedStandardWindowsFonts property
True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.
```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");
// Set PDF save options with EmbedStandardWindowsFonts property
PdfSaveOptions options = new PdfSaveOptions();
options.EmbedStandardWindowsFonts = true;
// Save to memory stream
using (MemoryStream ms = new MemoryStream())
{
workbook.Save(ms, options);
Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
}
// Demonstrate disabling font embedding
options.EmbedStandardWindowsFonts = false;
using (MemoryStream ms = new MemoryStream())
{
workbook.Save(ms, options);
Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
}
}
}
}
```
### See Also
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
