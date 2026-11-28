---
title: "Shape.FormatPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Resim biçiminin seçeneklerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

Resim biçiminin seçeneklerini alır ve ayarlar.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Şeklin FormatPicture özelliğine eriş
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // Resim biçimi özelliklerini değiştir
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


