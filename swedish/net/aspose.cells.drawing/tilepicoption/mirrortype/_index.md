---
title: "TilePicOption.MirrorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TilePicOption-egenskap. Hämtar eller anger spegeltyp för mosaik"
type: docs
url: /sv/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Hämtar eller anger spegeltypen för kakling.

```csharp
public MirrorType MirrorType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Ladda exempelbilddata (ersätt med faktisk bildsökväg)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // Skapa och konfigurera en TilePicOption‑instans
            TilePicOption tileOptions = new TilePicOption();

            // Visa initialt MirrorType-värde
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Konfigurera tile-alternativ
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Applicera Tile-konfiguration med korrekta egenskaper
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Spara den modifierade arbetsboken
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### Se även

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


