---
title: "Enum ColorDepth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.ColorDepth enum. Enumeriert den Bit-Tiefen-Typ für TIFF-Bilder"
type: docs
url: /de/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Enumeriert den Bit‑Tiefen‑Typ für TIFF‑Bilder.

```csharp
public enum ColorDepth
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Standardwert, nicht gesetzter Wert. |
| Format1bpp | `1` | 1 Bit pro Pixel |
| Format4bpp | `4` | 4 Bit pro Pixel |
| Format8bpp | `8` | 8 Bit pro Pixel |
| Format24bpp | `24` | 24 Bit pro Pixel |
| Format32bpp | `32` | 32 Bit pro Pixel |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // Konfiguriere TIFF-Bildoptionen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Render das Arbeitsblatt nach TIFF mit der angegebenen Farbtiefe
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Demonstriere eine weitere Farbtiefen-Variante
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


