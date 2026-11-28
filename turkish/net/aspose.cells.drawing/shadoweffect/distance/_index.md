---
title: "ShadowEffect.Distance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShadowEffect özelliği. Gölgenin mesafesini alır ve ayarlar. Aralık 0 ile 200 puan arasındadır"
type: docs
url: /tr/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Gölgenin mesafesini alır ve ayarlar. 0 ile 200 puan arasında.

```csharp
public double Distance { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dikdörtgen şekil ekleyin
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Gölge etkisini yapılandırın
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // CellsColor nesnesi oluşturun ve ARGB değerlerini ayarlayın
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Gölge mesafesini gösterin
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Gölge etkisiyle çalışma kitabını kaydedin
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


