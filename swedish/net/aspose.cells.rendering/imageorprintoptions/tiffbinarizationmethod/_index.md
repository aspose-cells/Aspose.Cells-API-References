---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger metod som används vid konvertering av bilder till 1 bpp-format när ImageType är Tiff och TiffCompression är lika med Ccitt3 eller Ccitt4"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

Hämtar eller anger metod som används vid konvertering av bilder till 1 bpp-format när [`ImageType`](../imagetype/) är Tiff och [`TiffCompression`](../tiffcompression/) är lika med Ccitt3 eller Ccitt4.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Anmärkningar

Standardvärdet är FloydSteinbergDithering.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // Skapa arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till gradientdata för visuell demonstration
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // Konfigurera TIFF-renderingsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Visa aktuell binariseringmetod
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Rendera med standardtröskelmetod
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Byt till Floyd-Steinberg-dithering
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Rendera med ny metod
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### Se även

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


