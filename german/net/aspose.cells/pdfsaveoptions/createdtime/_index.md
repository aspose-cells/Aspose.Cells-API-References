---
title: "PdfSaveOptions.CreatedTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Gibt die Erstellungszeit des PDF-Dokuments zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

Liest und setzt die Erstellungszeit des PDF-Dokuments.

```csharp
public DateTime CreatedTime { get; set; }
```

### Hinweise

Wenn sie nicht gesetzt ist, wird die Erstellungszeit des PDFs verwendet.

### Beispiele

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

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


