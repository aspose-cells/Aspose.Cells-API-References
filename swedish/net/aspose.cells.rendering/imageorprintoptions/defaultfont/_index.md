---
title: "ImageOrPrintOptions.DefaultFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. När tecken i Excel är Unicode och inte har rätt teckensnitt i cellstilen kan de visas som block i pdf-bild. Ange DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är satt kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken."
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är angiven kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode‑tecken.

```csharp
public string DefaultFont { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeltext i cellen
            worksheet.Cells["A1"].PutValue("Sample Text with Default Font");

            // Skapa bildalternativ och ange standardteckensnitt
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
            {
                DefaultFont = "Arial", // Setting default font
                ImageType = ImageType.Png
            };

            // Rendera kalkylblad till bild
            SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
            sheetRender.ToImage(0, "output.png");

            Console.WriteLine("Image generated with default font setting.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


