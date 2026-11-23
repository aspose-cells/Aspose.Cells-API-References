---
title: "Enum PdfCompliance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.PdfCompliance enum. Permet à l'utilisateur de définir la compatibilité des conversions PDF"
type: docs
url: /fr/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Permet à l'utilisateur de définir la compatibilité de la conversion PDF.

```csharp
public enum PdfCompliance
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Format PDF compatible avec PDF 1.4 |
| Pdf14 | `0` | Format PDF compatible avec PDF 1.4 |
| Pdf15 | `3` | Format PDF compatible avec PDF 1.5 |
| Pdf16 | `4` | Format PDF compatible avec PDF 1.6 |
| Pdf17 | `5` | Format PDF compatible avec PDF 1.7 |
| PdfA1b | `1` | Format PDF compatible avec PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | Format PDF compatible avec PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | Format PDF compatible avec PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | Format PDF compatible avec PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | Format PDF compatible avec PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | Format PDF compatible avec PDF/A-3b(ISO 19005-3) |
| PdfA3u | `10` | Format PDF compatible avec PDF/A-3u(ISO 19005-3) |
| PdfA3a | `11` | Format PDF compatible avec PDF/A-3a(ISO 19005-3) |

### Exemples

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
            // Création d'un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // Configuration des options d'enregistrement PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Définition du niveau de conformité à PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Enregistrement du classeur au format PDF avec le niveau de conformité spécifié
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


