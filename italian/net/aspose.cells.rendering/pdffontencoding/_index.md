---
title: "Enum PdfFontEncoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.PdfFontEncoding enum. Rappresenta la codifica dei font incorporati nel PDF"
type: docs
url: /it/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

Rappresenta la codifica del carattere incorporato pdf.

```csharp
public enum PdfFontEncoding
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Identity | `0` | Rappresenta l'uso della codifica Identity-H per tutti i font incorporati nel PDF. |
| AnsiPrefer | `1` | Rappresenta la preferenza di utilizzare WinAnsiEncoding per i font TrueType con caratteri da 32 a 127; altrimenti, verrà utilizzata la codifica Identity-H per i font incorporati nel PDF. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // Crea PdfSaveOptions e imposta la proprietà FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Salva la cartella di lavoro come file PDF
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


