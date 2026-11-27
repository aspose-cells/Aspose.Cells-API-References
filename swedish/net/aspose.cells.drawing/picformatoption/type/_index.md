---
title: "PicFormatOption.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PicFormatOption‑egenskap. Hämtar eller anger bildens fyllnadstyp"
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/type/
---
## PicFormatOption.Type property

Hämtar eller anger bildens fyllningstyp.

```csharp
public FillPictureType Type { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en enkel 1×1‑pixel BMP‑bild
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Lägg till bild i kalkylbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes));
            Picture picture = worksheet.Pictures[pictureIndex];

            // Ange bildens position och storlek
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 5;
            picture.LowerRightColumn = 5;

            try
            {
                // Hämta PicFormatOption från bildens texturfyllnad
                PicFormatOption picFormat = picture.Fill.TextureFill.PicFormatOption;

                // Visa det aktuella Type‑värdet
                Console.WriteLine("Current Type: " + picFormat.Type);

                // Ange olika Type‑värden och visa dem
                picFormat.Type = FillPictureType.Stretch;
                Console.WriteLine("Type set to Stretch: " + picFormat.Type);

                picFormat.Type = FillPictureType.Stack;
                Console.WriteLine("Type set to Stack: " + picFormat.Type);

                picFormat.Type = FillPictureType.StackAndScale;
                Console.WriteLine("Type set to StackAndScale: " + picFormat.Type);

                // Spara arbetsboken
                workbook.Save("PicFormatOptionTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [FillPictureType](../../fillpicturetype/)
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


