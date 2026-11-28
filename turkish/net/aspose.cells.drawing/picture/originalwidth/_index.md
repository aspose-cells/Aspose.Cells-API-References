---
title: "Picture.OriginalWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. Resmin orijinal genişliğini alır"
type: docs
url: /tr/net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Resmin orijinal genişliğini alır.

```csharp
public int OriginalWidth { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];

            // Resmin orijinal genişliğini al ve göster
            int originalWidth = pic.OriginalWidth;
            Console.WriteLine("Original width of the picture: " + originalWidth + " pixels");

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


