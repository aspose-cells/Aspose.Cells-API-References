---
title: "Enum TiffCompression"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.TiffCompression enum. Specifica il tipo di compressione da applicare quando si salvano immagini in un file TIFF"
type: docs
url: /it/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Specifica quale tipo di compressione applicare durante il salvataggio delle immagini in un file in formato TIFF.

```csharp
public enum TiffCompression
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| CompressionNone | `0` | Specifica nessuna compressione. |
| CompressionRle | `1` | Specifica lo schema di compressione RLE. |
| CompressionLZW | `2` | Specifica lo schema di compressione LZW. |
| CompressionCCITT3 | `3` | Specifica lo schema di compressione CCITT3. |
| CompressionCCITT4 | `4` | Specifica lo schema di compressione CCITT4. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingClassTiffCompressionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Imposta le opzioni dell'immagine
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Testa diversi tipi di compressione
            string outputPath = "output_compression_";

            // Compressione LZW
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // Compressione CCITT3
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // Compressione CCITT4
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


