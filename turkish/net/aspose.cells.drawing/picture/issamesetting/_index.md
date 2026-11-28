---
title: "Picture.IsSameSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture yöntemi. Şeklin aynı olup olmadığını döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Şeklin aynı olup olmadığını döndürür.

```csharp
public override bool IsSameSetting(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodIsSameSettingWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk resmi ekle (örnek bir görüntü yolu kullanarak)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // İkinci resmi ekle (farklı bir örnek görüntü yolu kullanarak)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Resmi kendisiyle karşılaştır
            if (pic1.IsSameSetting(pic1))
            {
                Console.WriteLine("pic1 and pic1 are the same");
            }
            
            // Farklı resimleri karşılaştır
            if (!pic1.IsSameSetting(pic2))
            {
                Console.WriteLine("pic1 and pic2 are different");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


