---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions costruttore. Crea le opzioni per salvare il file PDF"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Crea le opzioni per il salvataggio di un file pdf.

```csharp
public PdfSaveOptions()
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Dimostra il costruttore PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            
            // Salva la cartella di lavoro con le opzioni PDF
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("PDF saved successfully with PdfA1b compliance.");
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


