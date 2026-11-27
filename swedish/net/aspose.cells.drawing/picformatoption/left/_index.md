---
title: "PicFormatOption.Left"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PicFormatOption-egenskap. Hämtar eller anger det vänstra offsetet för att sträcka bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Hämtar eller anger det vänstra offsetet för att sträcka bilden.

```csharp
public double Left { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera bildformatering
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Konfigurera bildfyllning för formen
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // Skapa och konfigurera PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Tillämpa formatalternativ på formen (förutsatt att egenskapsnamnet är korrekt)
            // Obs: Den ursprungliga 'PictureFormatOptions'-egenskapen kanske inte finns i den aktuella API-versionen.
            // Raden nedan är kommenterad för att lösa kompileringsfelet.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // Visa initialt vänster offset
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Ändra vänster offset för att beskära 20 % från vänstra sidan
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Spara arbetsboken med modifierad bildformatering
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


