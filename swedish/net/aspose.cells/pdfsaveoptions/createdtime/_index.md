---
title: "PdfSaveOptions.CreatedTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions‑egenskap. Hämtar och anger tiden för generering av pdf‑dokumentet"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/createdtime/
---
## PdfSaveOptions.CreatedTime property

Hämtar och anger tiden för generering av pdf‑dokumentet.

```csharp
public DateTime CreatedTime { get; set; }
```

### Anmärkningar

Om den inte är angiven kommer den att vara tiden för generering av pdf‑dokumentet.

### Exempel

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

### Se även

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


