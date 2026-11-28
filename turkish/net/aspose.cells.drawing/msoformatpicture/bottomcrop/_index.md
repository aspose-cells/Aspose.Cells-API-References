---
title: "MsoFormatPicture.BottomCrop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kırpma dikdörtgeninin alt konumunu, görüntünün yüksekliğine oran olarak ifade eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/bottomcrop/
---
## MsoFormatPicture.BottomCrop property

Kırpma dikdörtgeninin alt konumunu, görüntünün yüksekliğine oran olarak ifade eder.

```csharp
public double BottomCrop { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPicturePropertyBottomCropDemo
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

            // Mevcut BottomCrop değerini göster
            Console.WriteLine("Current BottomCrop value: " + msoFormatPicture.BottomCrop);

            // Yeni bir BottomCrop değeri ayarla (0.2, alttan %20 kırpma anlamına gelir)
            msoFormatPicture.BottomCrop = 0.2;
            Console.WriteLine("BottomCrop set to: " + msoFormatPicture.BottomCrop);

            // Etkiyi göstermek için diğer kırpma değerlerini ayarla
            msoFormatPicture.TopCrop = 0.1;
            msoFormatPicture.LeftCrop = 0.1;
            msoFormatPicture.RightCrop = 0.1;

            // Kırpılmış resmi görmek için çalışma kitabını kaydet
            workbook.Save("MsoFormatPicturePropertyBottomCropDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


