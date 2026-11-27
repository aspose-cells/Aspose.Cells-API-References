---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar placeringen av vänster sida av beskärningsrektangeln uttryckt i tum"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Representerar platsen för den vänstra sidan av beskärningsrektangeln, uttryckt i tum.

```csharp
public double LeftCropInch { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Läs in bilddata
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Lägg till bild i kalkylbladet
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // Ange och hämta LeftCropInch‑egenskapen
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Spara arbetsboken
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


