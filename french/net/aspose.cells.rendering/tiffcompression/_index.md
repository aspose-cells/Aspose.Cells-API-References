---
title: "Enum TiffCompression"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.TiffCompression enum. Spécifie le type de compression à appliquer lors de l’enregistrement d’images au format TIFF"
type: docs
url: /fr/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Spécifie le type de compression à appliquer lors de l'enregistrement d'images au format TIFF.

```csharp
public enum TiffCompression
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| CompressionNone | `0` | Spécifie aucune compression. |
| CompressionRle | `1` | Spécifie le schéma de compression RLE. |
| CompressionLZW | `2` | Spécifie le schéma de compression LZW. |
| CompressionCCITT3 | `3` | Spécifie le schéma de compression CCITT3. |
| CompressionCCITT4 | `4` | Spécifie le schéma de compression CCITT4. |

### Exemples

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
            // Créez un nouveau classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Définissez les options d’image
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Testez différents types de compression
            string outputPath = "output_compression_";

            // Compression LZW
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // Compression CCITT3
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // Compression CCITT4
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


