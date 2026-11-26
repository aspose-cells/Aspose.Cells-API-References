---
title: "ImageOrPrintOptions.TiffCompression"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el tipo de compresión a aplicar solo al guardar páginas en formato Tiff"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/tiffcompression/
---
## ImageOrPrintOptions.TiffCompression property

Obtiene o establece el tipo de compresión que se aplicará solo al guardar páginas en el formato `Tiff`.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Observaciones

Tiene efecto solo al guardar en TIFF. El valor predeterminado es Lzw.

### Ejemplos

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
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Compression Test");

            // Establezca opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Pruebe diferentes tipos de compresión
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

### Ver también

* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


