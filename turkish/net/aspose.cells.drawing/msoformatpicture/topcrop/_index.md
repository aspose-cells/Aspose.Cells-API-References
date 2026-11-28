---
title: "MsoFormatPicture.TopCrop"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Kırpma dikdörtgeninin üst konumunu görüntünün yüksekliğine oran olarak ifade eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Kırpma dikdörtgeninin üst konumunu, görüntünün yüksekliğine oran olarak ifade eder.

```csharp
public double TopCrop { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir resim ekle
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // TopCrop özelliğini ayarla
            picture.FormatPicture.TopCrop = -6;
            
            // TopCrop değerini çıktı olarak ver
            Console.WriteLine("Picture TopCrop value: " + picture.FormatPicture.TopCrop);
            
            // Çalışma kitabını kaydedin
            workbook.Save("TopCropDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


