---
title: "ShadowEffect.Size"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShadowEffect özelliği. Gölgenin boyutunu alır ve ayarlar. Aralık 0 ile 2.0 arasındadır. İç gölgede anlamı yoktur"
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Gölgenin boyutunu alır ve ayarlar. Aralık 0 ile 2.0 arasındadır. İç gölgede anlamı yoktur.

```csharp
public double Size { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook book = new Workbook();
            
            // İlk çalışma sayfasına erişin ve bir şekil ekleyin
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Gölge etkisini alın ve Boyut dahil olmak üzere özellikleri ayarlayın
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Çalışma kitabını kaydedin
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


