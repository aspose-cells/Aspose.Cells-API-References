---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Bu resmin iki renkli siyah-beyaz olarak gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Bu resmin iki renkli siyah-beyaz olarak görüntülenip görüntülenmeyeceğini gösterir.

```csharp
public bool IsBiLevel { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
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
            
            // Resmi iki seviyeli (siyah beyaz) olarak ayarla
            picture.FormatPicture.IsBiLevel = true;
            
            // IsBiLevel özelliği değerini doğrulayın ve çıktısını alın
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


