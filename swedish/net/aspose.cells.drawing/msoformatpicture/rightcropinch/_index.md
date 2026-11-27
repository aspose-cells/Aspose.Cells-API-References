---
title: "MsoFormatPicture.RightCropInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture‑egenskap. Representerar placeringen av höger sida av beskärningsrektangeln uttryckt i tum"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/rightcropinch/
---
## MsoFormatPicture.RightCropInch property

Representerar platsen för den högra sidan av beskärningsrektangeln, uttryckt i tum.

```csharp
public double RightCropInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyRightCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en bild (ersätt med faktisk bildsökväg)
            int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Åtkomst och ange RightCropInch‑egenskapen
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.RightCropInch = 0.3; // Crop 0.3 inches from right

            // Spara arbetsboken
            workbook.Save("RightCropInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


