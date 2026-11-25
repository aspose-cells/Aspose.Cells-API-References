---
title: "PdfSaveOptions.Compliance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions property. Ottiene o imposta il livello di conformità agli standard PDF per i documenti di output"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Ottiene o imposta il livello di conformità agli standard PDF per i documenti di output.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Osservazioni

Il valore predefinito è Pdf17.

### Esempi

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
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // Imposta le opzioni di salvataggio PDF con conformità PDF/A-1b
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Salva la cartella di lavoro come PDF con impostazioni di conformità
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### Vedi anche

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


