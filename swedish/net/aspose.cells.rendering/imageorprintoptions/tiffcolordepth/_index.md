---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger bitdjup som endast ska tillämpas när sidor sparas i Tiff-formatet"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

Hämtar eller anger bithöjd att tillämpa endast när sidor sparas i `Tiff`-formatet.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Anmärkningar

Har effekt endast vid sparande till TIFF. Om TiffCompression är inställd på CCITT3, CCITT4, kommer detta inte att ha någon effekt, bitdjupet för den genererade tiff-bilden kommer alltid att vara 1.

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till formaterat innehåll för att demonstrera färgdjup
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // Initiera ImageOrPrintOptions för TIFF-rendering
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // Visa och ändra TiffColorDepth
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // Rendera med standarddjup (1bpp)
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // Ändra till 24-bitars färgdjup
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // Rendera med nytt djup
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### Se även

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


