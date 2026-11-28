---
title: "Shape.HeightScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Orijinal resim yüksekliğinin yüzde biriminde yükseklik ölçeğini alır ve ayarlar. Şekil resim değilse HeightScale özelliği yalnızca 100 döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Orijinal resim yüksekliğinin yüzde birimi cinsinden yükseklik ölçeğini alır ve ayarlar. Şekil resim değilse, HeightScale özelliği yalnızca 100 döndürür;

```csharp
public int HeightScale { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // İlk yükseklik ölçeğini ayarlayın
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Koşul karşılandığında yükseklik ölçeğini değiştirin
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


