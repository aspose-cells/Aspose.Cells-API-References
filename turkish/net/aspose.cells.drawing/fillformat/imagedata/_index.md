---
title: "FillFormat.ImageData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Resim veri bilgisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

Resim veri bilgisini alır ve ayarlar.

```csharp
public byte[] ImageData { get; set; }
```

### Açıklamalar

Doldurma formatı özel doku formatı değilse, null döndürür.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek resim ekle
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // Yorum oluştur ve resim verisini ayarla
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // Çalışma kitabını kaydet
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


