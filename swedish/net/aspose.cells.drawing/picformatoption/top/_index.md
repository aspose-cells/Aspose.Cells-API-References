---
title: "PicFormatOption.Top"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PicFormatOption-egenskap. Hämtar eller anger det övre offsetet för att sträcka bilden"
type: docs
url: /sv/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Hämtar eller anger det övre offsetet för att sträcka bilden.

```csharp
public double Top { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Använd en befintlig bild eller ange korrekt bildsökväg
            string imagePath = "existingImage.png";

            // Lägg till en form med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // Applicera bildfyllning med ImageData
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // Skapa och konfigurera PicFormatOption direkt
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // Antag att PicFormatOption måste associeras med fyllningsformatet
            // Denna del kan kräva API-specifik implementation som inte visas i typdefinitionerna
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### Se även

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


