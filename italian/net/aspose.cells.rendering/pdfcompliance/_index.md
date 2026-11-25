---
title: "Enum PdfCompliance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.PdfCompliance enum. Consente all'utente di impostare la compatibilità delle conversioni PDF"
type: docs
url: /it/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Consente all'utente di impostare la compatibilità della conversione PDF.

```csharp
public enum PdfCompliance
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Formato PDF compatibile con PDF 1.4 |
| Pdf14 | `0` | Formato PDF compatibile con PDF 1.4 |
| Pdf15 | `3` | Formato PDF compatibile con PDF 1.5 |
| Pdf16 | `4` | Formato PDF compatibile con PDF 1.6 |
| Pdf17 | `5` | Formato PDF compatibile con PDF 1.7 |
| PdfA1b | `1` | Formato PDF compatibile con PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | Formato PDF compatibile con PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | Formato PDF compatibile con PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | Formato PDF compatibile con PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | Formato PDF compatibile con PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | Formato PDF compatibile con PDF/A-3b(ISO 19005-3) |
| PdfA3u | `10` | Formato PDF compatibile con PDF/A-3u(ISO 19005-3) |
| PdfA3a | `11` | Formato PDF compatibile con PDF/A-3a(ISO 19005-3) |

### Esempi

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
            // Creazione di una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // Impostazione delle opzioni di salvataggio PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Impostazione del livello di conformità a PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Salvataggio della cartella di lavoro in PDF con il livello di conformità specificato
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


