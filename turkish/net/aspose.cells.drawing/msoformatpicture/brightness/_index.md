---
title: "MsoFormatPicture.Brightness"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Resmin parlaklık değişimini yüzde biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Resmin parlaklık değişimini yüzde biriminde temsil eder.

```csharp
public double Brightness { get; set; }
```

### Açıklamalar

-100% ile 100% arasında bir değerdir. Excel 2007 ve üzeri sürümlerle aynı şekilde çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBrightnessDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[pictureIndex];

            // Parlaklığı ayarla ve al
            picture.FormatPicture.Brightness = 30;
            Console.WriteLine("Picture brightness: " + picture.FormatPicture.Brightness);

            // Parlaklığı değiştir
            picture.FormatPicture.Brightness = 70;
            Console.WriteLine("Updated brightness: " + picture.FormatPicture.Brightness);
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


