---
title: "PdfSaveOptions.FontEncoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions Eigenschaft. Liest oder legt die eingebettete Schriftkodierung in PDF fest"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Liest oder setzt die eingebettete Schriftkodierung im PDF.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Hinweise

Standardwert ist Identity

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // Konfiguriere PDF-Speicheroptionen mit FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // Arbeitsmappe als PDF speichern
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


