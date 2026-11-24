---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt die Bit‑Tiefe zurück oder legt sie fest, die nur beim Speichern von Seiten im Tiff‑Format angewendet wird"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

Ruft die Bittiefe ab oder legt sie fest, die nur beim Speichern von Seiten im `Tiff`‑Format angewendet wird.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Hinweise

Wirkt nur beim Speichern als TIFF. Wenn TiffCompression auf CCITT3 oder CCITT4 gesetzt ist, hat dies keine Wirkung; die Bit‑Tiefe des erzeugten Tiff‑Bildes ist immer 1.

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formatierten Inhalt hinzufügen, um die Farbtiefe zu demonstrieren
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // ImageOrPrintOptions für die TIFF-Renderung initialisieren
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // TiffColorDepth anzeigen und ändern
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // Mit Standardtiefe (1bpp) rendern
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // Auf 24‑Bit‑Farbtiefe ändern
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // Mit neuer Tiefe rendern
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### Siehe auch

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


