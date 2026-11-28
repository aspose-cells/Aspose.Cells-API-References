---
title: "Picture.IsAutoSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. True, ole nesnesi etkinleştirildiğinde gömülü içeriğin anlık görüntüsü boyutuna göre nesnenin boyutunun otomatik olarak değiştirileceğini gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

True, OLE nesnesi etkinleştirildiğinde gömülü içeriğin anlık görüntüsü boyutuna göre OLE nesnesinin boyutunun otomatik olarak değişeceğini gösterir.

```csharp
public bool IsAutoSize { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // IsAutoSize özelliğini göster
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // IsAutoSize'ı true olarak ayarla - resim içeriğine sığacak şekilde otomatik olarak yeniden boyutlandırılacak
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // IsAutoSize'ı false olarak ayarla - resim özgün boyutlarını koruyacak
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Çalışma kitabını kaydedin
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


