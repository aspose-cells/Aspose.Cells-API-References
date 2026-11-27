---
title: "PdfSaveOptions.PdfCompression"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSaveOptions-egenskap. Anger komprimeringsalgoritmen"
type: docs
url: /sv/net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Ange komprimeringsalgoritmen

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyPdfCompressionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
            
            // Skapa PDF-sparalternativ med Flate-kompression
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            
            // Spara arbetsboken som PDF med kompression
            workbook.Save("output_with_flate_compression.pdf", saveOptions);
            
            // Spara igen utan kompression för jämförelse
            saveOptions.PdfCompression = PdfCompressionCore.None;
            workbook.Save("output_without_compression.pdf", saveOptions);
            
            Console.WriteLine("PDF files created successfully with different compression settings.");
        }
    }
}
```

### Se även

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


