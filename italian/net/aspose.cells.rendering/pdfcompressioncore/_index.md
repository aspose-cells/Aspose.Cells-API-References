---
title: "Enum PdfCompressionCore"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Rendering.PdfCompressionCore. Specifica un tipo di compressione applicata a tutti i contenuti nel file PDF, eccetto le immagini"
type: docs
url: /it/net/aspose.cells.rendering/pdfcompressioncore/
---
## PdfCompressionCore enumeration

Specifica un tipo di compressione applicato a tutti i contenuti del file PDF, eccetto le immagini.

```csharp
public enum PdfCompressionCore
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuno |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose!");

            // Crea PdfSaveOptions e imposta PdfCompressionCore
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Salva la cartella di lavoro come file PDF con la compressione specificata
            workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file saved with specified compression.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


