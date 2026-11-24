---
title: "PdfSaveOptions.PdfCompression"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions‑Eigenschaft. Gibt den Komprimierungsalgorithmus an"
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Gibt den Komprimierungsalgorithmus an

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
            
            // Erstellen Sie PDF‑Speicheroptionen mit Flate‑Kompression
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            
            // Speichern Sie die Arbeitsmappe als PDF mit Kompression
            workbook.Save("output_with_flate_compression.pdf", saveOptions);
            
            // Speichern Sie erneut ohne Kompression zum Vergleich
            saveOptions.PdfCompression = PdfCompressionCore.None;
            workbook.Save("output_without_compression.pdf", saveOptions);
            
            Console.WriteLine("PDF files created successfully with different compression settings.");
        }
    }
}
```

### Siehe auch

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


