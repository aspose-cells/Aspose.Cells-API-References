---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta la risoluzione orizzontale per le immagini generate in punti per pollice"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice.

```csharp
public int HorizontalResolution { get; set; }
```

### Osservazioni

Il valore predefinito è 96.

Impostare `HorizontalResolution` e [`VerticalResolution`](../verticalresolution/) influisce sulla larghezza e altezza dell'immagine di output in pixel.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // Inizializza ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Imposta la risoluzione orizzontale e verticale
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Esegui il rendering del foglio di lavoro in immagine con la risoluzione specificata
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Dimostra diverse risoluzioni
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


