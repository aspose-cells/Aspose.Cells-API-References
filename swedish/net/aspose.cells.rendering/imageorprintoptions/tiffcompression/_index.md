---
title: "ImageOrPrintOptions.TiffCompression"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Hämtar eller anger komprimeringstyp som endast tillämpas när sidor sparas i Tiff‑formatet"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/tiffcompression/
---
## ImageOrPrintOptions.TiffCompression property

Hämtar eller anger komprimeringstyp att tillämpa endast när sidor sparas i `Tiff`-formatet.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Anmärkningar

Har endast effekt vid sparande till TIFF. Standardvärdet är Lzw.

### Exempel

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
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Compression Test");

            // Ställ in bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Testa olika komprimeringstyper
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

### Se även

* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


