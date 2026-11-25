---
title: "PdfSaveOptions.PdfCompression"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Indica l'algoritmo di compressione"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Indica l'algoritmo di compressione

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample PDF Compression Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfCompression property usage");
            
            // Crea le opzioni di salvataggio PDF con compressione Flate
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            
            // Salva la cartella di lavoro come PDF con compressione
            workbook.Save("output_with_flate_compression.pdf", saveOptions);
            
            // Salva di nuovo senza compressione per il confronto
            saveOptions.PdfCompression = PdfCompressionCore.None;
            workbook.Save("output_without_compression.pdf", saveOptions);
            
            Console.WriteLine("PDF files created successfully with different compression settings.");
        }
    }
}
```

### Vedi anche

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


