---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions Eigenschaft. Gibt den PDF‑Standard‑Konformitätsgrad für Ausgabedokumente zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Liest oder setzt das PDF-Standardkonformitätsniveau für Ausgabedokumente.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Hinweise

Standard ist Pdf17.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyComplianceDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // PDF‑Speicheroptionen mit PDF/A‑1b‑Konformität festlegen
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Arbeitsmappe als PDF mit Konformitätseinstellungen speichern
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### Siehe auch

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


