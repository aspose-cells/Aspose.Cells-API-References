---
title: "ImageOrPrintOptions.TiffColorDepth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ImageOrPrintOptions property. Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato Tiff"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/tiffcolordepth/
---
## ImageOrPrintOptions.TiffColorDepth property

Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`.

```csharp
public ColorDepth TiffColorDepth { get; set; }
```

### Osservazioni

Ha effetto solo quando si salva in TIFF. Se TiffCompression è impostato su CCITT3, CCITT4, questo non avrà effetto; la profondità di bit dell'immagine TIFF generata sarà sempre 1.

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi contenuto formattato per dimostrare la profondità di colore
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("24-bit Color Depth");
            Style style = cell.GetStyle();
            style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
            style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
            style.Pattern = BackgroundType.Solid;
            cell.SetStyle(style);

            // Inizializza ImageOrPrintOptions per il rendering TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionLZW
            };

            // Visualizza e modifica TiffColorDepth
            Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
            
            // Esegui il rendering con profondità predefinita (1bpp)
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("DefaultDepthOutput.tiff");

            // Cambia a profondità di colore a 24 bit
            options.TiffColorDepth = ColorDepth.Format24bpp;
            Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");

            // Esegui il rendering con la nuova profondità
            renderer.ToTiff("24BitDepthOutput.tiff");

            Console.WriteLine("Generated TIFF files with different color depths.");
        }
    }
}
```

### Vedi anche

* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


