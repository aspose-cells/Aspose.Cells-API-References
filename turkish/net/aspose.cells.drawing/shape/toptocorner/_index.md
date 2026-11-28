---
title: "Shape.TopToCorner"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin çalışma sayfası üst kenarından piksel biriminde dikey ofsetini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Şeklin çalışma sayfasının üst kenarından dikey ofsetini piksel biriminde alır ve ayarlar.

```csharp
public int TopToCorner { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // TopToCorner özelliğini ayarlayın ve görüntüleyin
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // TopToCorner özelliğini değiştirin
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


