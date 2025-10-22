##Enum PdfCompliance
Aspose.Cells.Rendering.PdfCompliance enum. Allowing user to set PDF conversions Compatibility
## PdfCompliance enumeration
Allowing user to set PDF conversion's Compatibility
```csharp
public enum PdfCompliance
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Pdf format compatible with PDF 1.4 |
| Pdf14 | `0` | Pdf format compatible with PDF 1.4 |
| Pdf15 | `3` | Pdf format compatible with PDF 1.5 |
| Pdf16 | `4` | Pdf format compatible with PDF 1.6 |
| Pdf17 | `5` | Pdf format compatible with PDF 1.7 |
| PdfA1b | `1` | Pdf format compatible with PDF/A-1b(ISO 19005-1) |
| PdfA1a | `2` | Pdf format compatible with PDF/A-1a(ISO 19005-1) |
| PdfA2b | `6` | Pdf format compatible with PDF/A-2b(ISO 19005-2) |
| PdfA2u | `7` | Pdf format compatible with PDF/A-2u(ISO 19005-2) |
| PdfA2a | `8` | Pdf format compatible with PDF/A-2a(ISO 19005-2) |
| PdfA3b | `9` | Pdf format compatible with PDF/A-3b(ISO 19005-3) |
| PdfA3u | `10` | Pdf format compatible with PDF/A-3u(ISO 19005-3) |
| PdfA3a | `11` | Pdf format compatible with PDF/A-3a(ISO 19005-3) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PdfComplianceDemo
{
public static void PdfComplianceExample()
{
// Creating a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");
// Setting PDF save options
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Setting the compliance level to PDF/A-1b
saveOptions.Compliance = PdfCompliance.PdfA1b;
// Saving the workbook to PDF with the specified compliance level
workbook.Save("PdfComplianceExample.pdf", saveOptions);
Console.WriteLine("PDF generated with compliance level PDF/A-1b");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
