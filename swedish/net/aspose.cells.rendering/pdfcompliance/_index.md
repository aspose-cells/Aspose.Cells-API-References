---
title: "Enum PdfCompliance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfCompliance enum. Tillåter användaren att ställa in PDF-konverteringskompatibilitet"
type: docs
url: /sv/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Tillåter användaren att ställa in PDF‑konverteringens kompatibilitet.

```csharp
public enum PdfCompliance
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | PDF-format kompatibelt med PDF 1.4 |
| Pdf14 | `0` | PDF-format kompatibelt med PDF 1.4 |
| Pdf15 | `3` | PDF-format kompatibelt med PDF 1.5 |
| Pdf16 | `4` | PDF-format kompatibelt med PDF 1.6 |
| Pdf17 | `5` | PDF-format kompatibelt med PDF 1.7 |
| PdfA1b | `1` | PDF-format kompatibelt med PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | PDF-format kompatibelt med PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | PDF-format kompatibelt med PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | PDF-format kompatibelt med PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | PDF-format kompatibelt med PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | PDF-format kompatibelt med PDF/A-3b (ISO 19005-3) |
| PdfA3u | `10` | PDF-format kompatibelt med PDF/A-3u (ISO 19005-3) |
| PdfA3a | `11` | PDF-format kompatibelt med PDF/A-3a (ISO 19005-3) |

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // Ställa in PDF‑sparaalternativ
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Ställa in efterlevnadsnivån till PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Spara arbetsboken som PDF med den angivna efterlevnadsnivån
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


