---
title: "Klass PdfConverter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.PdfConverter-klass. Konverterare för att konvertera mallfil till pdf"
type: docs
url: /sv/net/aspose.cells.lowcode/pdfconverter/
---
## PdfConverter class

Konverterare för att konvertera mallfil till pdf.

```csharp
public class PdfConverter
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Konverterar mallfil till pdf |
| static [Process](../../aspose.cells.lowcode/pdfconverter/process/#process_1)(string, string) | Konverterar given mallfil till pdf. |

### Exempel

```csharp
using System;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassPdfConverterDemo
    {
        public static void Run()
        {
            // Initiera PdfConverter med mall- och utdatavägar
            PdfConverter.Process("template.xlsx", "res.pdf");
            
            Console.WriteLine("PDF conversion completed successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


