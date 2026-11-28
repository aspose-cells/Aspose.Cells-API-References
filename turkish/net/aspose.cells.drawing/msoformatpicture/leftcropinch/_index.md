---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kesme dikdörtgeninin sol konumunu inç birimiyle ifade eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

Kırpma dikdörtgeninin sol konumunu, inç cinsinden ifade eder.

```csharp
public double LeftCropInch { get; set; }
```

### Örnekler

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
            // Bir çalışma kitabı oluştur
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Görüntü verisini yükle
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Resmi çalışma sayfasına ekle
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // LeftCropInch özelliğini ayarla ve al
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // Çalışma kitabını kaydedin
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


