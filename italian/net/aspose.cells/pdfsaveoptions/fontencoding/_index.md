---
title: "PdfSaveOptions.FontEncoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Ottiene o imposta la codifica del font incorporato nel pdf"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Ottiene o imposta la codifica dei caratteri incorporati nel pdf.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Osservazioni

Il valore predefinito è Identity

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // Configura le opzioni di salvataggio PDF con FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // Salva la cartella di lavoro in PDF
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Vedi anche

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


