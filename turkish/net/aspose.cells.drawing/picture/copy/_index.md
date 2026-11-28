---
title: "Picture.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture yöntemi. Resmi kopyala"
type: docs
url: /tr/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Resmi kopyala.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Resim | Kaynak resim. |
| seçenekler | CopyOptions | Kopyalama seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodCopyWithPictureCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk resmi ekle (örnek bir görüntü yolu kullanarak)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // İkinci resmi ekle (örnek bir görüntü yolu kullanarak)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // CopyOptions ile resim 1'i resim 2'ye kopyala
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


