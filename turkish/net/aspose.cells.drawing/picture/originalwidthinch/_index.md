---
title: "Picture.OriginalWidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Picture özelliği. Resmin orijinal genişliğini inç biriminde alır"
type: docs
url: /tr/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

Resmin orijinal genişliğini inç biriminde alır.

```csharp
public double OriginalWidthInch { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir resim ekle ("example.jpg" yerine gerçek görüntü yolunuzu koyun)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // Orijinal genişliği inç cinsinden al ve göster
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


