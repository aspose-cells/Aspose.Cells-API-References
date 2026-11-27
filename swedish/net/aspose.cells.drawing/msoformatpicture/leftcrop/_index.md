---
title: "MsoFormatPicture.LeftCrop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture egenskap. Representerar placeringen av den vänstra sidan av beskärningsrektangeln uttryckt som en andel av bildens bredd"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Representerar platsen för den vänstra sidan av beskärningsrektangeln, uttryckt som en andel av bildens bredd.

```csharp
public double LeftCrop { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropDemo
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

            // Ställ in LeftCrop egenskap
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // Hämta och ställ in LeftCropInch egenskap
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Spara arbetsboken
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


