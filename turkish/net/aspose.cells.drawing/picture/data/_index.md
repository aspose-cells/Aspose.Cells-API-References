---
title: "Picture.Data"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture property. Resmin verisini alır"
type: docs
url: /tr/net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Resmin verilerini alır.

```csharp
public byte[] Data { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk resmi ekle
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // İkinci resmi ekle
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Veri özelliğini görüntü verisini kopyalayarak göster
            pic2.Data = pic1.Data;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


