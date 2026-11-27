---
title: "MsoFormatPicture.RightCrop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar platsen för den högra delen av beskärningsrektangeln uttryckt som en andel av bildens bredd"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Representerar platsen för den högra sidan av beskärningsrektangeln, uttryckt som en andel av bildens bredd.

```csharp
public double RightCrop { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Hämta MsoFormatPicture för bilden
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Visa det aktuella RightCrop‑värdet
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Ange ett nytt RightCrop‑värde (0,2 betyder beskärning med 20 % från höger)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Spara arbetsboken för att se effekten
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


