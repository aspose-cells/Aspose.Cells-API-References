---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Konstruktor. Erstellt die Optionen zum Speichern einer PDF-Datei."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Erstellt die Optionen zum Speichern einer PDF‑Datei.

```csharp
public PdfSaveOptions()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Demonstriere den PdfSaveOptions-Konstruktor.
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            
            // Speichere die Arbeitsmappe mit PDF-Optionen.
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("PDF saved successfully with PdfA1b compliance.");
        }
    }
}
```

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


