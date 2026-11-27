---
title: "MsoFormatPicture.BottomCrop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar platsen för den nedre delen av beskärningsrektangeln uttryckt som en andel av bildens höjd"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Representerar platsen för botten av beskärningsrektangeln, uttryckt som en andel av bildens höjd.

```csharp
public double BottomCrop { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
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

            // Visa det aktuella BottomCrop‑värdet
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Ange ett nytt BottomCrop‑värde (0,2 betyder beskärning med 20 % från botten)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Ange andra beskärningsvärden för att demonstrera effekten
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Spara arbetsboken för att se den beskurna bilden
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


