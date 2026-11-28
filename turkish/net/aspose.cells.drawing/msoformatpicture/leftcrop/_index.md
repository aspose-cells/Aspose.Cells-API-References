---
title: "MsoFormatPicture.LeftCrop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kırpma dikdörtgeninin sol konumunu, görüntünün genişliğine oran olarak temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/leftcrop/
---
## MsoFormatPicture.LeftCrop property

Kırpma dikdörtgeninin sol konumunu, görüntünün genişliğine oran olarak ifade eder.

```csharp
public double LeftCrop { get; set; }
```

### Örnekler

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
            // Bir çalışma kitabı oluştur
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // Görüntü verisini yükle
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // Resmi çalışma sayfasına ekle
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // LeftCrop özelliğini ayarla
            picture.FormatPicture.LeftCrop = 0.1;
            Console.WriteLine("LeftCrop set to: " + picture.FormatPicture.LeftCrop);

            // LeftCropInch özelliğini al ve ayarla
            double leftCropInch = picture.FormatPicture.LeftCropInch;
            picture.FormatPicture.LeftCropInch = leftCropInch;
            Console.WriteLine("LeftCropInch value: " + leftCropInch);

            // Çalışma kitabını kaydedin
            workbook.Save("LeftCropDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


