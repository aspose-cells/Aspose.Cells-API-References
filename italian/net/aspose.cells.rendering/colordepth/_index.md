---
title: "Enum ColorDepth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.ColorDepth enum. Enumera il tipo di profondità di bit per l'immagine tiff"
type: docs
url: /it/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Enumera il tipo di profondità di bit per le immagini tiff.

```csharp
public enum ColorDepth
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Valore predefinito, valore non impostato. |
| Format1bpp | `1` | 1 bit per pixel |
| Format4bpp | `4` | 4 bit per pixel |
| Format8bpp | `8` | 8 bit per pixel |
| Format24bpp | `24` | 24 bit per pixel |
| Format32bpp | `32` | 32 bit per pixel |

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // Configura le opzioni immagine TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Renderizza il foglio di lavoro in TIFF con la profondità di colore specificata
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Dimostra un'altra variante di profondità di colore
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


