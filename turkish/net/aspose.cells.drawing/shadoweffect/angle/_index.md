---
title: "ShadowEffect.Angle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShadowEffect özelliği. Aydınlatma açısını alır ve ayarlar. Aralık 0 ile 359.9 derece arasındadır"
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Aydınlatma açısını alır ve ayarlar. Aralık 0 ile 359,9 derece arasındadır.

```csharp
public double Angle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil ekleyin ve gölge etkisi açısını ayarlayın
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Açıyı doğrulayın ve değeri çıktı olarak verin
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


