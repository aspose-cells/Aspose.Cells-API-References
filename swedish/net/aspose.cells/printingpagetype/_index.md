---
title: "Enum PrintingPageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PrintingPageType‑enum. Anger vilka sidor som inte kommer att skrivas ut"
type: docs
url: /sv/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Anger vilka sidor som inte kommer att skrivas ut.

```csharp
public enum PrintingPageType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Skriver ut alla sidor. |
| IgnoreBlank | `1` | Skriv inte ut de sidor där cellerna är tomma. |
| IgnoreStyle | `2` | Skriv inte ut de sidor där cellerna bara innehåller format. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // Skapa PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Ställ in PrintingPageType till IgnoreBlank
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Spara arbetsboken som PDF med de angivna alternativen
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // Ställ in PrintingPageType till IgnoreStyle
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Spara arbetsboken som PDF med de angivna alternativen
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // Ställ in PrintingPageType till Default
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Spara arbetsboken som PDF med de angivna alternativen
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


