---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Hämtar eller anger PDF-standardens efterlevnadsnivå för utdata-dokument"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Hämtar eller anger PDF‑standardernas efterlevnadsnivå för utdata‑dokument.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Anmärkningar

Standard är Pdf17.

### Exempel

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
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // Ange PDF-sparalternativ med PDF/A-1b-efterlevnad
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Spara arbetsboken som PDF med efterlevnadsinställningar
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### Se även

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


