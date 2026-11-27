---
title: "Enum TiffCompression"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.TiffCompression-enum. Anger vilken typ av komprimering som ska tillämpas när bilder sparas i TIFF-formatfil"
type: docs
url: /sv/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Anger vilken typ av komprimering som ska tillämpas när bilder sparas i TIFF-formatfil.

```csharp
public enum TiffCompression
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| CompressionNone | `0` | Anger ingen komprimering. |
| CompressionRle | `1` | Anger RLE-komprimeringsschemat. |
| CompressionLZW | `2` | Anger LZW-komprimeringsschemat. |
| CompressionCCITT3 | `3` | Anger CCITT3-komprimeringsschemat. |
| CompressionCCITT4 | `4` | Anger CCITT4-komprimeringsschemat. |

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Ställ in bildalternativ
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Testa olika komprimeringstyper
            string outputPath = "output_compression_";

            // LZW-komprimering
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // CCITT3-komprimering
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // CCITT4-komprimering
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


