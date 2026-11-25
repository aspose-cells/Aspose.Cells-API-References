---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il metodo utilizzato durante la conversione delle immagini in formato 1 bpp quando ImageType è Tiff e TiffCompression è uguale a Ccitt3 o Ccitt4"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

Ottiene o imposta il metodo utilizzato durante la conversione delle immagini in formato 1 bpp quando [`ImageType`](../imagetype/) è Tiff e [`TiffCompression`](../tiffcompression/) è uguale a Ccitt3 o Ccitt4.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Osservazioni

Il valore predefinito è FloydSteinbergDithering.

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di gradiente per la dimostrazione visiva
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // Configura le opzioni di rendering TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Visualizza il metodo di binarizzazione corrente
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Esegui il rendering con il metodo di soglia predefinito
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Passa alla dithering Floyd-Steinberg
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Esegui il rendering con il nuovo metodo
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### Vedi anche

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


