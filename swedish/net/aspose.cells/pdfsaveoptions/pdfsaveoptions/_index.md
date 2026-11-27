---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-konstruktor. Skapar alternativ för att spara pdf‑fil"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Skapar alternativen för att spara pdf‑fil.

```csharp
public PdfSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Demonstrera PdfSaveOptions-konstruktor
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            
            // Spara arbetsboken med PDF‑alternativ
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("PDF saved successfully with PdfA1b compliance.");
        }
    }
}
```

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


