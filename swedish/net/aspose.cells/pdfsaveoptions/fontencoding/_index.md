---
title: "PdfSaveOptions.FontEncoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions egenskap. Hämtar eller sätter inbäddad teckenkodning i PDF"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Hämtar eller anger inbäddad teckenkodning i pdf.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Anmärkningar

Standardvärdet är Identity

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyFontEncodingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // Konfigurera PDF-sparalternativ med FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // Spara arbetsboken som PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


