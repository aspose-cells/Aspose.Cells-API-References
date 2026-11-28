---
title: "Picture.DisplayAsIcon"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture property. Belirtilen nesne simge olarak gösteriliyorsa ve görüntü otomatik olarak değiştirilmeyecekse doğru"
type: docs
url: /tr/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

Belirtilen nesne bir simge olarak görüntüleniyorsa ve resim otomatik olarak değişmeyecekse true.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekle
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // DisplayAsIcon özelliğini doğru olarak ayarla
            picture.DisplayAsIcon = true;
            
            // Diğer resim özelliklerini ayarla
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Çalışma kitabını kaydedin
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


