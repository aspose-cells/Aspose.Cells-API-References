---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin orijinal resim boyutuna göre göreli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

Şeklin orijinal resim boyutuna göre relatif olup olmadığını gösterir.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Şekil özelliklerine erişin - Picture zaten bir Shape, dönüştürmeye gerek yok
            Shape shape = picture;

            // RelativeToOriginalPictureSize özelliğini gösterin
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // Özelliği değiştir
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


