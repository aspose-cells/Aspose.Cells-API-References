---
title: "MsoFormatPicture.TopCropInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kırpma dikdörtgeninin üst konumunu inç biriminde ifade eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

Kırpma dikdörtgeninin üst konumunu, inç cinsinden ifade eder.

```csharp
public double TopCropInch { get; set; }
```

### Örnekler

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

            // Bir resim ekleyin (gerçek görüntü yoluyla değiştirin)
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // TopCropInch özelliğine erişin ve değiştirin
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // Sonucu kaydet
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


