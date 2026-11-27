---
title: "LowCodePdfSaveOptions.PdfOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodePdfSaveOptions egenskap. Alternativen för att spara Pdf-fil"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/
---
## LowCodePdfSaveOptions.PdfOptions property

Alternativen för att spara PDF-fil.

```csharp
public PdfSaveOptions PdfOptions { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodePdfSaveOptionsPropertyPdfOptionsDemo
    {
        public static void Run()
        {
            // Skapa exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Options Demo");

            // Skapa PDF-sparalternativ med anpassade inställningar
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b,
                OnePagePerSheet = true
            };

            // Skapa lågkod PDF-sparalternativ och tilldela PDF-alternativen
            LowCodePdfSaveOptions lowCodePdfSaveOptions = new LowCodePdfSaveOptions
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfSaveOptions
            };

            // Spara med lågkodalternativ
            workbook.Save(lowCodePdfSaveOptions.OutputFile, lowCodePdfSaveOptions.PdfOptions);

            Console.WriteLine("PDF saved with custom options.");
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


