---
title: "ImageOrPrintOptions.Quality"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna och som endast tillämpas när sidor sparas i Jpeg‑formatet. Standardvärdet är 100"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Hämtar eller anger ett värde som bestämmer kvaliteten på de genererade bilderna, som endast tillämpas när sidor sparas i `Jpeg`‑formatet. Standardvärdet är 100.

```csharp
public int Quality { get; set; }
```

### Anmärkningar

Har endast effekt när du sparar till JPEG. Värdet måste vara mellan 0 och 100. Standardvärdet är 100.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Skapa bildalternativ med olika kvalitetsinställningar
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Rendera kalkylblad till bild med hög kvalitet
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Ändra kvalitet för att demonstrera skillnad
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


