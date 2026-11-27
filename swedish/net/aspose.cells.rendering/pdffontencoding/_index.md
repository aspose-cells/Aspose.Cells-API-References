---
title: "Enum PdfFontEncoding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfFontEncoding enum. Representerar inbäddad teckenkodning för pdf"
type: docs
url: /sv/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

Representerar inbäddad PDF-teckensnittskodning.

```csharp
public enum PdfFontEncoding
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Identity | `0` | Representerar användning av Identity-H‑kodning för alla inbäddade teckensnitt i pdf. |
| AnsiPrefer | `1` | Representerar föredraget att använda WinAnsiEncoding för TrueType‑teckensnitt med tecken 32‑127, annars kommer Identity-H‑kodning att användas för inbäddade teckensnitt i pdf. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // Skapa PdfSaveOptions och ställ in egenskapen FontEncoding
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Spara arbetsboken som en PDF-fil
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


