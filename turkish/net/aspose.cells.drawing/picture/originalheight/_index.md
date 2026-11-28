---
title: "Picture.OriginalHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture property. Resmin orijinal yüksekliğini alır"
type: docs
url: /tr/net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Resmin orijinal yüksekliğini alır.

```csharp
public int OriginalHeight { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];

            // Resmin orijinal yüksekliğini al ve göster
            int originalHeight = pic.OriginalHeight;
            Console.WriteLine("Original height of the picture: " + originalHeight + " pixels");

            // Çalışma kitabını kaydedin
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


