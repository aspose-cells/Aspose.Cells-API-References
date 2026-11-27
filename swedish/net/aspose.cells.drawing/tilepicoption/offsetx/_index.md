---
title: "TilePicOption.OffsetX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TilePicOption-egenskap. Hämtar eller anger X‑förskjutningen för mosaikbild"
type: docs
url: /sv/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Hämtar eller anger X‑förskjutningen för kakelbilden.

```csharp
public double OffsetX { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel för att demonstrera mosaik
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Konfigurera fyllningsformatet för att använda en kaklad bild
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Skapa och konfigurera TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Läs initialt OffsetX‑värde
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Ange ny X‑förskjutning för mosaikmönster
            tileOptions.OffsetX = 15.5;

            // Tillämpa kakelalternativ på formens fyllning
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Läs in minimal 1x1‑pixelbild (röd prick)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Spara modifierad arbetsbok
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### Se även

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


