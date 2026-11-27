---
title: "MsoFormatPicture.TopCrop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture-egenskap. Representerar platsen för den övre delen av beskärningsrektangeln uttryckt som en andel av bildens höjd"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Representerar platsen för den övre delen av beskärningsrektangeln, uttryckt som en andel av bildens höjd.

```csharp
public double TopCrop { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en bild i arbetsbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Ställ in TopCrop-egenskap
            picture.FormatPicture.TopCrop = -6;
            
            // Skriv ut TopCrop-värdet
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Spara arbetsboken
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


