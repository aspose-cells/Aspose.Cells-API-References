---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger den horisontella upplösningen för genererade bilder i punkter per tum"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Hämtar eller anger den horisontella upplösningen för genererade bilder, i punkter per tum.

```csharp
public int HorizontalResolution { get; set; }
```

### Anmärkningar

Standardvärdet är 96.

Att ställa in `HorizontalResolution` och [`VerticalResolution`](../verticalresolution/) påverkar bredden och höjden på den genererade bilden i pixlar.

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // Initiera ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Ställ in horisontell och vertikal upplösning
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Rendera kalkylbladet till bild med angiven upplösning
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Demonstrera olika upplösningar
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


