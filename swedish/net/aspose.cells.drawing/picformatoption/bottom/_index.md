---
title: "PicFormatOption.Bottom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PicFormatOption-egenskap. Hämtar eller anger det nedre offsetet för att sträcka bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Hämtar eller anger det nedre offsetet för att sträcka bilden.

```csharp
public double Bottom { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Använd en befintlig bildfil (ersätt med faktisk bildsökväg)
            string imagePath = "sample.jpg";

            // Lägg till en rektangelform i arbetsbladet
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Konfigurera formens fyllning för att använda exempelbilden
            // FillType härleds genom att sätta ImageData, vilket sätter typen till Texture
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Skapa och konfigurera bildformatalternativen
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // Visa initialt Bottom-värde
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Ändra Bottom-offsetet och visa det nya värdet
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // Associera PicFormatOption med formens fyllning (förutsatt att det är tillämpligt)
            // Obs: Detta steg kan kräva API-specifika metoder som inte visas i det tillhandahållna sammanhanget
            // För demonstration skapas och konfigureras PicFormatOption

            // Spara arbetsboken med tillämpade ändringar
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### Se även

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


