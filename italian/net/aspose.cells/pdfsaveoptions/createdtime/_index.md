---
title: "PdfSaveOptions.CreatedTime"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSaveOptions property. Ottiene e imposta il tempo di generazione del documento pdf"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

Ottiene o imposta l'ora di generazione del documento pdf.

```csharp
public DateTime CreatedTime { get; set; }
```

### Osservazioni

se non è impostato, sarà il tempo di generazione del pdf.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("PDF with CreatedTime demonstration");

            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                CreatedTime = DateTime.Now,
                Compliance = PdfCompliance.PdfA1b
            };

            string outputPath = "OutputWithCreatedTime.pdf";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine($"PDF saved with CreatedTime: {saveOptions.CreatedTime}");
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


