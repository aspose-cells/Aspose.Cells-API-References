---
title: "ShadowEffect.Blur"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShadowEffect özelliği. Gölgenin bulanıklığını alır ve ayarlar. Aralık 0 ile 100 puan arasındadır"
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Gölgenin bulanıklığını alır ve ayarlar. 0 ile 100 puan arasında.

```csharp
public double Blur { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyBlurDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Gölge etkisini alın
            ShadowEffect shadow = shape.ShadowEffect;
            
            // Bulanıklık dahil olmak üzere gölge özelliklerini ayarlayın
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4;
            shadow.Distance = 80;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Shadow effect with blur applied successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


