---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt die Methode zum Konvertieren von Bildern in das 1-bpp-Format zurück oder legt sie fest, wenn ImageType Tiff ist und TiffCompression gleich Ccitt3 oder Ccitt4 ist"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

Gibt die Methode zurück oder legt sie fest, die beim Konvertieren von Bildern in das 1-bpp-Format verwendet wird, wenn [`ImageType`](../imagetype/) Tiff ist und [`TiffCompression`](../tiffcompression/) gleich Ccitt3 oder Ccitt4 ist.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Hinweise

Der Standardwert ist FloydSteinbergDithering.

### Beispiele

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
            // Arbeitsmappe mit Beispieldaten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Verlaufsdaten für die visuelle Demonstration hinzu
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // Konfigurieren Sie die TIFF-Renderoptionen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Aktuelle Binärisierungsmethode anzeigen
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Rendern mit der Standard-Schwellenwertmethode
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Wechseln zu Floyd-Steinberg-Dithering
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Rendern mit neuer Methode
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### Siehe auch

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


