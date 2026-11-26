---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece la profundidad de bits que se aplicará solo al guardar páginas en formato Tiff"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

Obtiene o establece la profundidad de bits que se aplicará solo al guardar páginas en el formato `Tiff`.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Observaciones

Tiene efecto solo al guardar en TIFF. Si TiffCompression está configurado a CCITT3 o CCITT4, no tendrá efecto; la profundidad de bits de la imagen TIFF generada será siempre 1.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyTiffColorDepthDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue contenido formateado para demostrar la profundidad de color
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // Inicialice ImageOrPrintOptions para el renderizado TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // Muestre y modifique TiffColorDepth
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // Renderice con la profundidad predeterminada (1bpp)
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // Cambie a una profundidad de color de 24 bits
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // Renderice con la nueva profundidad
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### Ver también

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


