---
title: "MsoFormatPicture.TopCropInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFormatPicture-egenskap. Representerar platsen för den övre delen av beskärningsrektangeln uttryckt i tum"
type: docs
url: /sv/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Representerar platsen för den övre delen av beskärningsrektangeln, uttryckt i tum.

```csharp
public double TopCropInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en bild (ersätt med faktisk bildsökväg)
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // Åtkomst och ändra TopCropInch-egenskap
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // Spara resultatet
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


