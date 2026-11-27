---
title: "PdfSaveOptions.DisplayDocTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Anger om fönstrets titelrad ska visa dokumenttiteln"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Anger om fönstrets titellist ska visa dokumenttiteln.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Anmärkningar

Om falskt ska titelraden istället visa namnet på PDF-filen. Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyDisplayDocTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF DisplayDocTitle Example");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Ställ in egenskapen DisplayDocTitle till true
            pdfSaveOptions.DisplayDocTitle = true;

            // Spara arbetsboken som PDF
            workbook.Save("PdfDisplayDocTitleDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


