---
title: "Enumeración TiffCompression"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Rendering.TiffCompression enum. Especifica qué tipo de compresión aplicar al guardar imágenes en un archivo de formato TIFF"
type: docs
url: /es/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Especifica qué tipo de compresión aplicar al guardar imágenes en un archivo de formato TIFF.

```csharp
public enum TiffCompression
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| CompressionNone | `0` | Especifica sin compresión. |
| CompressionRle | `1` | Especifica el esquema de compresión RLE. |
| CompressionLZW | `2` | Especifica el esquema de compresión LZW. |
| CompressionCCITT3 | `3` | Especifica el esquema de compresión CCITT3. |
| CompressionCCITT4 | `4` | Especifica el esquema de compresión CCITT4. |

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Establezca opciones de imagen
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Pruebe diferentes tipos de compresión
            string outputPath = "output_compression_";

            // Compresión LZW
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // Compresión CCITT3
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // Compresión CCITT4
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


