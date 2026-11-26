---
title: "Enum ColorDepth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Rendering.ColorDepth enum. Enumera el tipo de profundidad de bits para imágenes tiff"
type: docs
url: /es/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Enumera el tipo de profundidad de bits para imágenes TIFF.

```csharp
public enum ColorDepth
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Valor predeterminado, valor no establecido. |
| Format1bpp | `1` | 1 bit por píxel |
| Format4bpp | `4` | 4 bits por píxel |
| Format8bpp | `8` | 8 bits por píxel |
| Format24bpp | `24` | 24 bits por píxel |
| Format32bpp | `32` | 32 bits por píxel |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class RenderingClassColorDepthDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // Configurar opciones de imagen TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Renderizar la hoja de cálculo a TIFF con la profundidad de color especificada
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Demostrar otra variante de profundidad de color
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


