---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar platsen för den nedre delen av beskärningsrektangeln uttryckt i tum"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Representerar platsen för den nedre delen av beskärningsrektangeln, uttryckt i tum.

```csharp
public double BottomCropInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en bild i kalkylbladet (med en platshållar‑sökväg)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Åtkomst till MsoFormatPicture‑objektet
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Ange BottomCropInch‑egenskapen och demonstrera dess användning
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Spara arbetsboken
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


