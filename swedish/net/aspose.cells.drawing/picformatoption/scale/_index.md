---
title: "PicFormatOption.Scale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PicFormatOption-egenskap. Hämtar eller anger hur många bilden staplar och skalar med"
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/scale/
---
## PicFormatOption.Scale property

Hämtar eller anger hur många bildstackar och skalningsfaktor som används.

```csharp
public double Scale { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO; // Added to resolve Stream-related issues

    public class PicFormatOptionPropertyScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en 1×1 pixel BMP-bild som byte-array
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Lägg till bilden i kalkylbladet med MemoryStream
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes)); // Fixed Stream conversion
            Picture picture = worksheet.Pictures[pictureIndex];

            // Konfigurera bildens position och storlek
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 1;
            picture.LowerRightColumn = 1;

            // Hämta texturfyllning via FillFormat-egenskapen
            TextureFill textureFill = picture.Fill.TextureFill; // Fixed cast error
            textureFill.PicFormatOption.Type = FillPictureType.Stack;

            // Visa och ändra Scale-egenskapen
            PicFormatOption picFormat = textureFill.PicFormatOption;
            Console.WriteLine("Current Scale value: " + picFormat.Scale);
            picFormat.Scale = 0.5;
            Console.WriteLine("Modified Scale value: " + picFormat.Scale);

            // Expandera cellens dimensioner för att visualisera effekten
            worksheet.Cells.SetRowHeight(0, 100);
            worksheet.Cells.SetColumnWidth(0, 20);

            // Spara arbetsboken
            workbook.Save("PropertyScaleDemo.xlsx");
        }
    }
}
```

### Se även

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


