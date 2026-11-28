---
title: "ShadowEffect.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShadowEffect özelliği. Gölgenin şeffaflık derecesini alır ve ayarlar. 0.0 opakdan 1.0 tamamen şeffafa kadar aralık"
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Gölgenin şeffaflık derecesini alır ve ayarlar. Aralık 0.0 (opak) ile 1.0 (şeffaf) arasındadır.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gölge etkisini göstermek için bir şekil ekleyin
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Gölge etkisini alın ve Şeffaflık dahil olmak üzere özellikleri ayarlayın
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3;
            shadow.Transparency = 0.4; // Setting transparency to 40%
            shadow.Distance = 80;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShadowEffectDemo.xlsx");
            
            Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


