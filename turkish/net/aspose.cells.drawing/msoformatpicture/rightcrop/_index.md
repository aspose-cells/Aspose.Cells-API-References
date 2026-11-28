---
title: "MsoFormatPicture.RightCrop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kırpma dikdörtgeninin sağ konumunu, görüntünün genişliğine oran olarak ifade eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/rightcrop/
---
## MsoFormatPicture.RightCrop property

Kırpma dikdörtgeninin sağ konumunu, görüntünün genişliğine oran olarak ifade eder.

```csharp
public double RightCrop { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyRightCropDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Resmin MsoFormatPicture öğesini al
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;

            // Mevcut RightCrop değerini göster
            Console.WriteLine("Current RightCrop value: " + msoFormatPicture.RightCrop);

            // Yeni bir RightCrop değeri ayarla (0.2, sağdan %20 kırpma anlamına gelir)
            msoFormatPicture.RightCrop = 0.2;
            Console.WriteLine("New RightCrop value set to: " + msoFormatPicture.RightCrop);

            // Etkiyi görmek için çalışma kitabını kaydet
            workbook.Save("RightCropDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


