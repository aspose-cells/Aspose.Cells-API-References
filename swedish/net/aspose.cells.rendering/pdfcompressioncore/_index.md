---
title: "Enum PdfCompressionCore"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfCompressionCore enum. Anger en typ av kompression som tillämpas på allt innehåll i PDF‑filen förutom bilder"
type: docs
url: /sv/net/aspose.cells.rendering/pdfcompressioncore/
---
## PdfCompressionCore enumeration

Specificerar en komprimeringstyp som tillämpas på allt innehåll i PDF‑filen förutom bilder.

```csharp
public enum PdfCompressionCore
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCompressionCoreDemo
    {
        public static void PdfCompressionCoreExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose!");

            // Skapa PdfSaveOptions och ange PdfCompressionCore
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Spara arbetsboken som en PDF-fil med den angivna komprimeringen
            workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file saved with specified compression.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


