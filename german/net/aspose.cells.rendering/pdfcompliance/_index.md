---
title: "Enum PdfCompliance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfCompliance enum. Ermöglicht dem Benutzer, die Kompatibilität von PDF-Konvertierungen festzulegen"
type: docs
url: /de/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Ermöglicht dem Benutzer, die Kompatibilität der PDF-Konvertierung festzulegen.

```csharp
public enum PdfCompliance
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | PDF-Format kompatibel mit PDF 1.4 |
| Pdf14 | `0` | PDF-Format kompatibel mit PDF 1.4 |
| Pdf15 | `3` | PDF-Format kompatibel mit PDF 1.5 |
| Pdf16 | `4` | PDF-Format kompatibel mit PDF 1.6 |
| Pdf17 | `5` | PDF-Format kompatibel mit PDF 1.7 |
| PdfA1b | `1` | PDF-Format kompatibel mit PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | PDF-Format kompatibel mit PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | Pdf-Format kompatibel mit PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | Pdf-Format kompatibel mit PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | Pdf-Format kompatibel mit PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | Pdf-Format kompatibel mit PDF/A-3b (ISO 19005-3) |
| PdfA3u | `10` | Pdf-Format kompatibel mit PDF/A-3u (ISO 19005-3) |
| PdfA3a | `11` | Pdf-Format kompatibel mit PDF/A-3a (ISO 19005-3) |

### Beispiele

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
            // Erstellen einer Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // Einstellen der PDF‑Speicheroptionen
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Festlegen des Konformitätslevels auf PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Speichern der Arbeitsmappe als PDF mit dem angegebenen Konformitätslevel
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


