---
title: "ImageOrPrintOptions.TiffCompression"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato Tiff"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/tiffcompression/
---
## ImageOrPrintOptions.TiffCompression property

Ottiene o imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Osservazioni

Ha effetto solo quando si salva in TIFF. Il valore predefinito è Lzw.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTiffCompressionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Compression Test");

            // Imposta le opzioni dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Testa diversi tipi di compressione
            string outputPath = "OutputTIFF_";

            options.TiffCompression = TiffCompression.CompressionNone;
            SaveAsTiff(workbook, options, outputPath + "None.tiff");

            options.TiffCompression = TiffCompression.CompressionRle;
            SaveAsTiff(workbook, options, outputPath + "Rle.tiff");

            options.TiffCompression = TiffCompression.CompressionLZW;
            SaveAsTiff(workbook, options, outputPath + "LZW.tiff");

            options.TiffCompression = TiffCompression.CompressionCCITT3;
            SaveAsTiff(workbook, options, outputPath + "CCITT3.tiff");

            options.TiffCompression = TiffCompression.CompressionCCITT4;
            SaveAsTiff(workbook, options, outputPath + "CCITT4.tiff");
        }

        private static void SaveAsTiff(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            renderer.ToImage(fileName);
        }
    }
}
```

### Vedi anche

* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


