---
title: "Enum ColorDepth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.ColorDepth‑enum. Enumererar bitdjupstyp för tiff‑bild"
type: docs
url: /sv/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Enumererar bitdjupstyp för TIFF‑bild.

```csharp
public enum ColorDepth
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Standardvärde, ej angivet värde. |
| Format1bpp | `1` | 1 bit per pixel |
| Format4bpp | `4` | 4 bitar per pixel |
| Format8bpp | `8` | 8 bitar per pixel |
| Format24bpp | `24` | 24 bitar per pixel |
| Format32bpp | `32` | 32 bitar per pixel |

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // Konfigurera TIFF‑bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Rendera arbetsblad till TIFF med angivet färgdjup
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Demonstrera en annan färgdjupvariant
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


