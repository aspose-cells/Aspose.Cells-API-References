---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kırpma dikdörtgeninin alt konumunu inç birimiyle ifade eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

Kırpma dikdörtgeninin alt konumunu, inç cinsinden ifade eder.

```csharp
public double BottomCropInch { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle (yer tutucu yol kullanarak)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // MsoFormatPicture nesnesine erişin
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // BottomCropInch özelliğini ayarla ve kullanımını göster
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // Çalışma kitabını kaydedin
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


